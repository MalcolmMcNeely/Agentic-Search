---
name: team-comp
description: Build a five-hero AFK Journey comp from the roster and the fight, then reconcile it against ./account/teams.md. Fires when the user asks for a team for a mode, boss, tower or event, asks to swap a hero into a comp, or asks whether a comp still holds up.
---

# Team comp

Two moves, in this order. **Draft** five heroes from the account and the fight. **Reconcile** the draft against [account/teams.md](../../../account/teams.md), which is where it becomes a new comp, a replacement, or a confirmation of the one already fielded.

Drafting first is what gives the reconcile its worth. A comp built from the roster and the rules alone either agrees with the file, or names a reason the file should change.

## Draft

1. **Name the fight.** Which mode, boss, tower or event, and what does it field against the user? Read that mode's file in `mechanics/`; [game-modes.md](../../../mechanics/game-modes.md) lists them all. When the user leaves the mode open, ask one short question, because the mode's rules decide every choice below.

2. **Read what the account can field.** [roster.md](../../../account/roster.md) for heroes, tiers and EX. [progression.md](../../../account/progression.md) for Resonance Level, Hands and artifacts owned. [equipment.md](../../../account/equipment.md) for class gear and charms. These three files set the ceiling.

3. **Build the five.** Follow [team-building.md](../../../mechanics/team-building.md) in the order it states. [team-archetypes.md](../../../mechanics/team-archetypes.md) picks the pattern the five run on. Open a hero's file from [heroes/README.md](../../../mechanics/heroes/README.md) whenever its kit decides a slot.

   **Every eligible hero on the roster is a candidate.** Start from the whole roster and cut it down with the fight's rules, rather than starting from the heroes a guide happens to name. A hero is dropped for a reason read off its kit, never for being absent from a tier list. [hero-scoring.md](../../../mechanics/hero-scoring.md) is the method, and the guide silence rule there says why this step exists.

4. **Place and kit it.** Rows from [formation.md](../../../mechanics/formation.md). One artifact from [artifacts.md](../../../mechanics/artifacts.md), at a level `progression.md` says is owned.

   **Place every entity, not every hero.** A five-hero comp is rarely five tiles. Elijah & Lailah deploy as two bodies, Phraesto stands beside an Illusion, and Taichi & Agumon puts only Agumon on the grid. **State the count hero by hero**, because it is a property of the hero, not of the comp, and give each entity its own row. Name the summons and zones that arrive later too, wherever their position changes what they are worth. The full table is in [formation.md](../../../mechanics/formation.md).

5. **Assign the Hands of Resonance, but only if the slots differ.** The account owns five levelled **slots**, not five levelled heroes. `progression.md` holds the slot levels; read them there rather than from here, because they move. Swapping a hero into a slot is free, unlimited, and the level travels with the slot, so any comp can hold all five. See [progression-systems.md](../../../mechanics/progression-systems.md).

   - **Never write a level next to a hero, and never add a Level column.** The level belongs to the slot, so a level beside a hero is stale the moment the user rearranges the Resonating Hall. `progression.md` records the Resonance Level once, and that is the only level in the repo.
   - **Read `progression.md` first, then decide whether there is anything to say.** When every slot stands level with the Resonance Level, the comp says **nothing** about levels: there is no choice to make.
   - **When one slot stands above the others, name the hero that should hold it.** Put it where 10 levels pay most, which is the carry first, then the hero that must survive for the pattern to work. Say it in the comp, because the swap happens before the fight.
   - **Pick the comp on its kits, then hand it the slots.** Every comp can hold all five, so the assignment follows the comp rather than choosing it.

   The Resonance Level is the **lowest** slot, so it never moves when heroes change slots. It moves only when a slot's level changes.

Done when five heroes are named, each confirmed in `roster.md` at the tier claimed, **every entity each hero fields counted and placed in a row**, one artifact named at an owned level, no level written beside any hero, and one line saying what each hero is there to do.

## Reconcile

5. **Open [teams.md](../../../account/teams.md) and find the purpose.** Four branches:

   | The file holds | Do this |
   | --- | --- |
   | no comp for this purpose | Write the draft in as a new comp, status `proposed`. |
   | the same five as the draft | Say the file already holds it. Correct any detail that drifted: a tier, an artifact level, a row. |
   | a different comp, status `proposed` | Replace it in place. The reason goes in the commit message. |
   | a different comp, status `running` | Set the draft beside the running comp for the user and let them pick. The user fields `running` comps in game. |

6. **Settle a clash.** The draft may rest on a fact that `teams.md` states differently, such as a hero tier or an artifact level. `roster.md`, `progression.md` and `equipment.md` decide it, and the file that was wrong gets corrected in the same turn.

7. **Name the shared heroes.** A hero in the draft may already stand in another comp in the file. Say which comps move together, so a fix in one stays a fix in both.

8. **Write it down.** Follow the rules at the top of `teams.md`: one comp per purpose, replace in place, present tense, and the `> **Updated:**` line refreshed. A comp that reaches the user in chat alone is lost by the next session, which then invents a different one.

9. **Hand it over.** Name the files the comp came from. A fact carrying a `?`, `unverified` or `disputed` marker keeps that marker in the answer.

Done when the purpose holds exactly one comp, every hero in it matches `roster.md`, any clash is settled in both files, and the user knows which other comps share a hero with it.

## Gaps

A fact the draft needs that no file holds is a gap. The `lookup` skill sorts it: a game rule goes to `game-research`, and anything only the user knows goes to them as one short question.
