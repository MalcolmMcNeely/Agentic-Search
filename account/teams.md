# Teams

> **Covers:** the current team comp for each purpose, its formation, artifact and status.
> **Updated:** 2026-08-29

One comp per purpose. This file holds what to field **now**, not how the advice got here.

Git holds the history. A comp that is replaced is **deleted** from this file, and the reason goes in the commit message. Never keep a dead comp for the record.

## How to change a comp

1. **Read the comps here first.** A new one either fills an empty purpose or replaces the comp already holding it.
2. **Replace in place.** Delete the old comp, write the new one, and say why in the commit message.
3. **Never replace a `running` comp without the user.** `running` means they field it in game. Propose the change and let them decide.
4. **Check every hero against [roster.md](roster.md)** at the tier claimed, before writing the comp down.
5. **Date it,** so the next session can judge the comp rather than guess at it.

## Status

| Status | Meaning |
| --- | --- |
| `running` | the user fields this in game |
| `proposed` | recommended here, not yet confirmed in game |
| `blocked` | a hero is missing |

---

## AFK Stages, main — Lightbearer Resonance — `running` 2026-08-29

**Purpose:** AFK Stages and campaign.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Temesia | Lightbearer | 1 |
| Middle | Aurora | Celestial | 2 |
| Back | Hugin | Lightbearer | 20 |
| Back | Zanie | Lightbearer | 20 |
| Back | Rolan | Celestial | 10 |

**Artifact:** Confining Spell +6.

**Why:** two engines at once. Rolan clones an ally Ultimate, and opens with a Morale spike that **doubles to 10% per hero** because Lightbearer is the most-deployed faction. Aurora raises the damage of every allied summon, and Zanie, Temesia and Aurora all field summons. Three Lightbearers plus two wildcarding Celestials pay the **+22%** cap, plus +1% per Celestial. No other comp on this account reaches +22%.

**Three weak points:**

1. **One payload, four engines.** [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md) calls Rolan and Aurora engines, not carries. Hugin is support, Temesia is a tank. **Zanie** is the only real damage dealer.
2. **No healer.** Hugin gives cogshields and damage reduction. Rolan heals only as Morale climbs. Nothing heals on demand.
3. **One hero at the level cap.** Only Hugin is a Hand of Resonance at 120. Temesia, Aurora, Zanie and Rolan sit at 110. Swapping a Hand is free, so this is fixable. See [../mechanics/progression-systems.md](../mechanics/progression-systems.md).

**Risk:** Aurora is an engine at range 2, so she has to come forward. Confining Spell is picked to keep enemies off her.

**First swap to try if it stalls:** Temesia out, **Solise** in, for healing and a team damage buff. It drops the core to 2 Lightbearer, so the bonus falls to +14%, and it leaves no tank. Test it, do not assume it.

**Open test:** Starshard fires every 4 ally Ultimates, and Rolan's clones cast Ultimates. If clones feed the counter, Starshard may beat Confining here. Unknown.

---

## AFK Stages, backup — Shemira scaling carry — `running` 2026-08-29

**Purpose:** the saved second formation, for fights where the main comp's frontline collapses.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Thador | Wilder | 1 |
| Middle | Daimon | Graveborn | 3 |
| Middle | Shemira | Graveborn | 4 |
| Back | Bonnie | Graveborn | 7 |
| Back | Hugin | Lightbearer | 20 |

**Artifact:** Confining Spell +6. Faction bonus **+10%**, from 3 Graveborn.

**Why:** long AFK fights suit a scaling carry. Shemira snowballs and heals off her own ghosts, Daimon shields, Bonnie strips enemy Haste and ATK, Thador tanks and heals. Hugin is the one Hand at 120 and buffs the carry's ATK and Haste directly. This comp has a real tank *and* real shielding, which the main comp does not.

**Grid note:** keep Thador on the tile between Shemira and the enemy backline. She carries at range 4 and gets reached without him.

**Eironn is deliberately out.** His pull only fires at battle start from **Mythic+**. He is Epic.

**Upgrade when owned:** Ulmus replaces Thador. He is the named tank for this pattern and is A-Level, so he comes off the **All-Hero** wishlist, never an Epic letter. See [../mechanics/recruitment.md](../mechanics/recruitment.md).

---

## PvP — Eironn nuke — `blocked` on ascension

**Purpose:** Arena, and any fight where enemies stand in a group.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Thador | Wilder | 1 |
| Middle | Eironn | Wilder | 1 |
| Middle | Faramor | Wilder | 1 |
| Back | Solise | Wilder | 6 |
| Back | Aurora | Celestial | 2 |

**Artifact:** Confining Spell +6.

**Why:** Eironn's Ultimate drags every enemy within 2 tiles into one pile, freezes them 3s and cuts their Magic DEF by 40%. Faramor's circle punishes the stack and blocks enemy healing. Four Wilders plus Aurora wildcarding = **+22%**.

**Blocked on Eironn reaching Mythic+.** Only then does his Ultimate fire at battle start. He is Epic. Until then the pull is not guaranteed to land first and the comp is a worse version of itself. Copies are the unlock.

**Swap:** Arden for Faramor once Arden is above Elite. He charges his Ultimate off Eironn's hit and is the named payload for this pattern.

---

## Dream Realm, Snow Stomper — `proposed` 2026-08-29

**Purpose:** the Snow Stomper boss only. See [../mechanics/snow-stomper.md](../mechanics/snow-stomper.md).

| Role | Hero | Faction | Range |
| --- | --- | --- | --- |
| DPS carry | Galahad | Mauler | 10 |
| Debuffer | Kruger | Mauler | 1 |
| Healer | Smokey & Meerky | Mauler | 8 |
| Buffer | Hugin | Lightbearer | 20 |
| Flex | Taichi & Agumon | Dimensional | 7, then 1 |

**Artifact:** Starshard Spell +5. True damage ignores the boss's defence.

**Why:** fills the four roles the guides agree on. Galahad's Time Recast makes another hero fire again, which is the whole point of a single-target damage race. Kruger and Taichi & Agumon are the only heroes this account owns that the Snow Stomper guides name. Three Maulers pay **+10%**.

**Known compromise:** the boss's frontal Frost cone punishes melee, and both Kruger and the digivolved Taichi & Agumon end up at range 1. They are in for their kits, not their positioning.

---

## Purposes with no comp yet

Arcane Labyrinth, Legend Trial, Battle Drills, Supreme Arena. Legend Trial is faction-locked and needs a mono-faction build, so it will not reuse any comp above. See [../mechanics/legend-trial.md](../mechanics/legend-trial.md).

## Onward

- Which heroes are owned and at what tier: [roster.md](roster.md)
- Why a comp is shaped this way: [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md)
- The order to build a new one in: [../mechanics/team-building.md](../mechanics/team-building.md)
- Rows and range: [../mechanics/formation.md](../mechanics/formation.md)
