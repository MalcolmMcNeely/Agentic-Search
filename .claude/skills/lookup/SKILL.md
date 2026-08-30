---
name: lookup
description: Read INDEX.md and follow its pointers before answering any AFK Journey question. Fires on a request for a team comp, a hero, a faction, a game mode, an in-game event, or the state of the account.
---

# Lookup

The repo is the memory. `INDEX.md` is the way in. Nothing here is loaded until a pointer sends you to it, so an answer written without reading the files is a guess.

Retrieval has two moves. **Follow** a pointer when you know which file holds the answer. **Grep** when you do not. Both beat reading everything.

## Steps

1. **Read [INDEX.md](../../../INDEX.md).** Always, first, before any other tool call.

2. **Match the triggers.** Each index line ends in a `read it when` clause. Read every file whose clause matches the question. Reading one extra file is cheap; skipping one is a wrong answer.

3. **Take the second hop.** Some pointers lead to another index rather than an answer. `mechanics/heroes/README.md` is the big one: 40 hero files behind one line. Read its table, then open only the hero files the answer needs.

4. **Grep when the question cuts across files.** Hero files carry the same five fields, so a set question is one command, not 40 reads:

   ```bash
   grep -l "Class:\*\* Tank" mechanics/heroes/*.md
   grep -rl "Damage:\*\* Magic" mechanics/heroes/
   grep -rn "Confining" account/ mechanics/
   ```

   Grep to find the files, then read them. Never answer from the grep line alone.

5. **Follow the onward pointers.** Files link to each other. Keep following until the links stop telling you anything new.

6. **Name the gaps.** A **gap** is a fact the question needs that no file holds. Sort each gap:
   - A game rule, hero kit, artifact or event detail is a research gap. Invoke the `game-research` skill.
   - Anything only the user can know, such as what they own, what they cleared, or what the event screen says, is an account gap. Ask them, in one short question.

7. **Hand a team comp to the `team-comp` skill.** It owns the order: draft the five from `account/roster.md` and `mechanics/`, then reconcile against `account/teams.md` and write the result there.

8. **Answer from the files.** Say which files the answer came from. When a fact carries a `?`, `unverified` or `disputed` marker in its source file, say so in the answer rather than smoothing it over.

Done when every matching pointer has been read, every cross-file set was found by grep rather than by guessing, every gap is either researched or put to the user, and any team comp request has been passed to the `team-comp` skill.

## The pointer contract

Three rules keep the lookup working:

- Every file under `account/` and `mechanics/` opens with a `> **Covers:**` line. That line is the file's own claim about itself, and its index line should say the same thing.
- Every hero file carries the same five fields, in the same order, so grep finds sets across the folder.
- A file that no index line names is unreachable. The skills that write files also write the index line. See `account-update` and `game-research`, and run `audit` to catch drift.

## The known failure mode

Runtime exploration goes wrong by chasing dead ends: opening files the question never needed, or wandering the folder instead of reading the index. The index exists to make that unnecessary. Read it first, match the triggers, and stop when the question is answered.
