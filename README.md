# Agentic search

A working example of retrieval without a vector database.

The repo manages my AFK Journey account. That is the real job it does. It is also a demonstration of **agentic search**, the pattern Claude Code uses instead of RAG. The agent holds file paths and index lines rather than embeddings, reads an index, decides what it needs, and opens only those files.

[RAG-ALTERNATIVE.md](RAG-ALTERNATIVE.md) is the write-up. It names the pattern, gives the benchmark numbers on both sides, lists what it costs, and points at the file here that demonstrates each part.

## It only works under certain conditions

This is not a better RAG. It is a trade, and it goes bad outside its range.

It wins when:

- the corpus is small enough for an agent to navigate by hand, roughly tens of files, not millions
- the facts change often, so a stale embedding would be worse than no embedding
- a human needs to read and correct the stored facts
- latency does not matter, because the agent explores at question time

It loses when:

- the corpus is large. RAG keeps the speed win at 100 documents and pulls ahead on accuracy by 1000.
- an answer has to arrive in under a second, such as a customer-facing search box
- nobody is maintaining the index. Nothing enforces it but discipline.

LlamaIndex measured both over five arXiv papers. The filesystem agent scored 8.4/10 on correctness against RAG's 6.4, and took 11.17s against RAG's 7.36s. Better answers, slower. That is the whole trade in one row.

## How to read it

| Path | What it is |
| --- | --- |
| [CLAUDE.md](CLAUDE.md) | the always-loaded layer, kept tiny on purpose |
| [INDEX.md](INDEX.md) | the index. One line per file: `path — what it holds — read it when` |
| [RAG-ALTERNATIVE.md](RAG-ALTERNATIVE.md) | the write-up on the pattern |
| `account/` | facts about one player, changing weekly |
| `mechanics/` | facts about the game, changing on patch days |
| `.claude/skills/` | the four procedures: lookup, account-update, game-research, audit |

The `read it when` clause in INDEX.md is the part doing the work an embedding would do. The agent matches the question against that clause instead of against a similarity score.

## What is missing from the clone

My raw notes file is gitignored. It is an unfiled inbox of account data, superseded by everything in `account/`, and it would only mislead you.
