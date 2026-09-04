# What this repo is, as a retrieval pattern

> **Covers:** the name of the pattern this repo uses instead of a vector database, what it costs, what it buys, and which file does which job.
> **Updated:** 2026-08-29

This repo manages an AFK Journey account. It is also a worked example of a retrieval pattern that replaces RAG, so this file explains the pattern and points at the parts of the repo that demonstrate it.

## The name

There is no single agreed name. The same pattern is published under all of these:

| Name | Who uses it |
| --- | --- |
| **Agentic search**, or **agentic retrieval** | Anthropic, Elastic, most engineering write-ups |
| **Just-in-time context loading** | Anthropic's context engineering post |
| **Agent-as-retriever** | academic and vendor write-ups |
| **Vectorless RAG**, **embedding-free RAG** | the contrast-with-RAG framing |
| **Filesystem tools**, **file search** | LlamaIndex benchmarks, OpenAI tooling |

**Agentic search** is the most used, and **just-in-time context loading** is the most descriptive. This document uses agentic search.

## What it replaces

Classic RAG runs a fixed pipeline before the model ever speaks. Chunk the corpus, embed every chunk, store the vectors, embed the question, pull the top k chunks by similarity, paste them into the prompt. Retrieval happens once, before generation, and the model has no say in it.

Agentic search deletes that pipeline. The agent holds **lightweight identifiers** instead: file paths, index lines, links. It reads an index, decides what it needs, opens those files, and can go back for more. Anthropic describes agents that "maintain lightweight identifiers (file paths, stored queries, web links, etc.) and use these references to dynamically load data into context at runtime using tools."

Retrieval stops being a pipeline stage and becomes a behaviour: the agent decides what to look for, when to look again, and when to stop.

## Why anyone bothers

Claude Code shipped with the classic version and threw it away. Boris Cherny, who created it, said early versions used RAG with a local vector database, but "agentic search generally works better. It is also simpler and doesn't have the same issues around security, privacy, staleness, and reliability."

The benchmarks back the quality claim and puncture the speed claim.

LlamaIndex ran both over five arXiv papers with five question-answer pairs each:

| | Filesystem agent | RAG |
| --- | --- | --- |
| Correctness | **8.4** / 10 | 6.4 / 10 |
| Relevance | **9.6** / 10 | 8.0 / 10 |
| Time | 11.17s | **7.36s** |

Scaled to 100 papers, then 1000, RAG kept the speed win and pulled ahead slightly on correctness. The crossover is real: agentic search wins on small corpora, RAG wins on large ones.

A second test, on FinanceBench with table-heavy filings, gave a keyword-search agent 30.40% answer correctness against RAG's 24.24%, same model and same context window, the retriever being the only difference.

## Pros

- **No pipeline.** No embedding model, no chunk size, no vector store, no re-indexing job. A text editor is the whole write path.
- **No chunking loss.** The agent reads whole files. RAG hands over fragments torn out of their context, which is exactly why it loses on tables and cross-referenced documents.
- **No staleness.** The files are the source of truth, not a copy of it. A vector store holds embeddings without timestamps, so a fact embedded six months ago scores the same as one embedded today. Editing a file here changes the answer immediately.
- **Human-readable and human-writable.** You can read, correct and diff every stored fact. You cannot read an embedding.
- **The agent can change its mind mid-task.** It refines the query, follows a link, and goes back for more. One-shot retrieval cannot.
- **Simpler security and privacy.** There is no second copy of the data sitting in a vector database.
- **Structure carries meaning.** Folder and file names are signals. Anthropic's example: `test_utils.py` in `tests/` means something different from the same filename in `src/core_logic/`. Naming does work that an embedding cannot.

## Cons

- **Slower.** Runtime exploration beats precomputed lookup on quality and loses on latency. Fine for a chat about a game, wrong for a customer-facing search box.
- **It does not scale.** RAG handles millions of documents and billions of embeddings. This pattern handles what an agent can navigate by hand. Once tuned, RAG tackles greater complexity than a filesystem agent.
- **Token cost per question is higher**, because the agent explores instead of issuing one query. The counter-argument is real but partial: you spend tokens only on what the agent judged relevant and skip everything else.
- **The index is maintained by hand.** Filesystem storage has "weak concurrency, manual schema enforcement" and no transactions. Nothing stops a file drifting out of sync with its index line except discipline.
- **The agent can chase dead ends.** Anthropic names this directly: it takes careful engineering to stop agents "misusing tools, chasing dead-ends, or failing to identify key information."
- **Quality is entirely a function of file hygiene.** Bad files give bad answers, with no similarity score to hide behind.

## The honest verdict

Agentic search is not strictly better than RAG. It wins where the corpus is small, the facts change often, a human needs to read and correct them, and latency does not matter. It loses where the corpus is huge and the answer has to arrive in under a second.

An account of 37 heroes and a dozen rule files is squarely in the first case.

## How this repo demonstrates it

Every part of the pattern has a file here.

### The always-loaded layer

[CLAUDE.md](CLAUDE.md) is dropped into context at the start of every session, unread by choice. It is deliberately tiny: the layout, the rules, and one pointer to the index. This is the hybrid Anthropic describes, where "CLAUDE.md files are naively dropped into context up front, while primitives like glob and grep allow it to navigate its environment and retrieve files just-in-time."

### The index

[INDEX.md](INDEX.md) is the store of lightweight identifiers. One line per file, in the form `path — what it holds — read it when`.

The `read it when` clause is the working part. It is a **context pointer**: it names material and encodes the condition for reaching it. The agent matches the question against the clause, not against a similarity score. This is what replaces the embedding.

### The second hop

37 hero files would bloat the index into something nobody reads. So `mechanics/heroes/README.md` is a second index, and INDEX.md spends one line pointing at it.

This is **progressive disclosure**: the index stays legible, and the 37 files stay one hop away instead of loaded. The cost is one extra read when a hero is actually needed. Anthropic's framing is that agents "incrementally discover relevant context through exploration."

### Grep as the second retrieval move

Following a pointer works when you know which file holds the answer. When you do not, grep does the job an embedding search would have done.

Every hero file carries the same five fields in the same order, so a set question is one command:

```bash
grep -l "Class:\*\* Tank" mechanics/heroes/*.md
grep -rl "Damage:\*\* Magic" mechanics/heroes/
```

The fixed field format is not decoration. It is the schema that makes keyword retrieval work across 37 files, and it is the "manual schema enforcement" the criticism warns about, done on purpose.

### Naming as signal

`account/` holds what is true about one player and changes weekly. `mechanics/` holds how the game works and changes on patch days. `account/roster.md` and `mechanics/heroes/cecia.md` both describe Cecia, and the paths say which one is a fact about the player and which is a fact about the game. No embedding conveys that. The folder name does it for free.

### The skills

The four skills in `.claude/skills/` are the behaviour half of the pattern. Retrieval and writing are things the agent does, so they are written down as procedures rather than left to chance.

| Skill | Invocation | Job |
| --- | --- | --- |
| `lookup` | model | read the index, match triggers, take the second hop, grep for sets, name the gaps |
| `account-update` | model | file a new fact into `account/`, run the consistency checks, refresh the index line |
| `game-research` | model | fill a gap from the web into `mechanics/`, with sources, then refresh the index line |
| `audit` | user | sweep for unreachable files, dead links, broken contracts and drift |

`lookup` also carries the named failure mode, so the agent knows what going wrong looks like: chasing dead ends instead of reading the index first.

`audit` exists because of a specific documented weakness. The index is maintained by hand and nothing enforces it, so the mitigation is a sweep the human can run on demand. It is user-invoked, which means it has no description in the agent's context and costs nothing until typed.

### Freshness beats similarity

The rule in [CLAUDE.md](CLAUDE.md) that **the account beats the guides** is the staleness advantage made concrete.

It has already fired once. Several published guides state that equipment cannot exceed a player's Resonance Level. This account runs Resonance Level 220 with sixteen gear slots at 240. The observed fact won, the rule is marked `disputed` in [mechanics/equipment-and-charms.md](mechanics/equipment-and-charms.md), and the reason is written next to it.

A vector store would have returned the guide's claim with a high similarity score and no way to notice it was wrong.

## Sources

- https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents
- https://www.llamaindex.ai/blog/did-filesystem-tools-kill-vector-search
- https://buzzgrewal.medium.com/ai-agents-dont-need-vector-search-anymore-inside-the-agentic-search-stack-replacing-rag-in-2026-58efcabe4f6f
- https://www.elastic.co/search-labs/blog/search-tools-context-engineering
- https://www.algolia.com/blog/ai/agentic-retrieval
- https://towardsdatascience.com/beyond-rag/
- https://robertheubanks.substack.com/p/anthropic-replaced-their-rag-pipeline
