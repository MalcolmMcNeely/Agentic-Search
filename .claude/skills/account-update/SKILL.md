---
name: account-update
description: Record a change to the AFK Journey account into ./account. Fires when the user reports pulling or ascending a hero, a Resonance Level or Hands of Resonance change, new gear, artifacts or charms, or progress in a game mode. Also fires when the user says they updated the notes file.
---

# Account update

The user speaks in fragments, or dumps raw lines into the `notes` inbox at the repo root. "Got Lyca", "Cecia is epic+ now", "cleared 600". The job is to turn each fragment into a row that a future team-comp answer can trust.

## Steps

1. **Read the inbox and the target file.** Check `notes` for anything not yet filed. Then pick the target:
   - [account/roster.md](../../../account/roster.md) for heroes.
   - [account/teams.md](../../../account/teams.md) for a comp the user adopts, drops, or reports a result for. Read its rules before writing: one comp per purpose, replace in place, and never replace a `running` comp without asking the user.
   - [account/progression.md](../../../account/progression.md) for Resonance Level, Hands, power, artifacts owned, mode progress.
   - [account/equipment.md](../../../account/equipment.md) for class gear, EX weapons, charms.

   Read the target before editing, so the existing columns and faction groupings survive.

2. **Fill in what the user left out.** A hero named for the first time needs a faction and a class before it can go in a table. Look it up with the `game-research` skill rather than guessing, and write `?` in any cell still unknown after research.

3. **Write the change.** Keep the row in its faction section, keep the column order, and update the `> **Updated:**` date at the top of the file. Update the faction depth counts in `roster.md` when a hero is added or removed.

4. **Run the consistency checks.** Each is a real game rule, so a failure means the record is wrong or the user misspoke. Report a failure to the user, do not silently correct it.
   - The Resonance Level equals the **lowest** Hand of Resonance level.
   - No Hand exceeds the Resonance Level by more than 10.
   - There are exactly five Hands of Resonance.
   - Every Hand appears in `roster.md` too, at the same tier.
   - Ascension tiers come from the list in [mechanics/progression-systems.md](../../../mechanics/progression-systems.md). Rare heroes cannot ascend.
   - Any per-class gear average matches the six slot numbers it summarises.

5. **Catch the guides being wrong.** New account numbers that break a rule written in `mechanics/` mean the guide is stale. Mark that rule `disputed` in its mechanics file and name what the account shows. See the rule in [CLAUDE.md](../../../CLAUDE.md).

6. **Refresh [INDEX.md](../../../INDEX.md)** if a file now covers something its index line does not describe. A new file always needs a new index line.

Done when every fact the user stated appears in a file, all consistency checks pass or are reported, any stale mechanics rule is marked, and the index describes what the files now hold.

## When research is worth it

Record first, research second. A tier bump on a hero already in the table needs no web search. A hero the roster has never seen does, because faction and class decide every future comp it appears in.
