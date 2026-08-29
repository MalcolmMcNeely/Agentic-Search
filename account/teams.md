# Teams

> **Covers:** every team comp built for this account, what each is for, and which are actually in use.
> **Updated:** 2026-08-29

Comps accumulate here. Several sessions write to this file, and they will disagree, so the rules below keep the disagreement readable instead of destructive.

## How to add a comp

1. **Read every comp already here first.** A new one either fills an empty purpose or supersedes an existing comp.
2. **Supersede, do not overwrite.** Move the old comp to `superseded`, keep it in place, and say in one line what the new comp does better. A comp is only deleted when the account can no longer field it.
3. **Only one comp per purpose holds `running` or `proposed`.** Two live comps for the same mode means the reconciliation was skipped.
4. **Check every hero against [roster.md](roster.md)** at the tier claimed, before writing the comp down.
5. **Sign it.** Every comp carries the date and the reason it was picked, so the next session can judge it rather than guess.

## Status

| Status | Meaning |
| --- | --- |
| `running` | the user actually fields this |
| `proposed` | recommended here, not yet confirmed in game |
| `blocked` | a hero is missing |
| `superseded` | kept for the record, replaced by a named comp |

---

## Levelling default — `superseded` 2026-08-29

**Superseded by Lightbearer Resonance**, which the user confirmed running on 2026-08-29. It trades the +10 levels on four Hands for the +22% faction cap and two engines.

**Purpose:** whatever the five levelled heroes can carry. Not a designed comp.

Taichi & Agumon, Yamato & Gabumon, Hugin, Pandora, Daimon

These are the five Hands of Resonance, the only heroes above the Resonance Level. See [progression.md](progression.md). Faction bonus is **+10%**, from 3 Dimensional.

**Why it is weak:** Hugin and Daimon add nothing to the faction bonus. Any comp below beats it on paper but fields heroes ten levels lower.

**The fix is levelling, not swapping.** Daimon is the lowest Hand at 110 and sets the Resonance Level. Taking him to 120 lifts every other hero on the account from 110 to 120, which makes every comp below live.

---

## Lightbearer Resonance — `running` 2026-08-29

Confirmed by the user on 2026-08-29: this is the comp being fielded for AFK battles. It supersedes the Levelling default.

**Purpose:** AFK Stages and campaign. The best comp the account can field once levels are even.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Temesia | Lightbearer | 1 |
| Middle | Aurora | Celestial | 2 |
| Back | Hugin | Lightbearer | 20 |
| Back | Zanie | Lightbearer | 20 |
| Back | Rolan | Celestial | 10 |

**Artifact:** Confining Spell +6.

**Why:** two engines at once. Rolan clones an ally Ultimate, and opens with a Morale spike that **doubles to 10% per hero** because Lightbearer is the most-deployed faction. Aurora buffs every allied summon, and Zanie, Temesia and Aurora all field summons. Three Lightbearers plus two wildcarding Celestials pay the **+22%** cap, plus +1% per Celestial.

**Risk:** Aurora is the engine and sits at range 2, so she has to come forward. Confining Spell is picked to keep enemies off her.

**Open test:** Starshard fires every 4 ally Ultimates, and Rolan's clones cast Ultimates. If clones feed the counter, Starshard may beat Confining here. Unknown.

**Three weak points, reviewed 2026-08-29.** The faction and kit maths above check out against [../mechanics/factions.md](../mechanics/factions.md), [roster.md](roster.md) and the hero files. These are the costs it pays:

1. **One payload, four engines.** [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md) calls Rolan and Aurora engines, not carries. Hugin is support and Temesia is a tank. That leaves **Zanie** as the only real damage dealer, rated A+ for campaign. If Zanie stalls, nothing else replaces her damage.
2. **No healer.** Hugin gives cogshields and damage reduction. Rolan heals only as Morale climbs. Nothing here heals on demand. The account's real healers are Hewynn and Solise, both Wilder, and neither fits the Lightbearer core.
3. **One hero at the level cap.** Only Hugin is a Hand of Resonance at 120. Temesia, Aurora, Zanie and Rolan all sit at 110. Swapping a Hand is free, so this is fixable. See [../mechanics/progression-systems.md](../mechanics/progression-systems.md) and [progression.md](progression.md).

**First swap to try if it stalls:** Temesia out, **Solise** in. Solise heals in waves and her Bulbsprites raise team damage. It drops the core to 2 Lightbearer, so the bonus falls from +22% to +14%, and it removes the only tank. Test it, do not assume it.

---

## Eironn nuke — `proposed` 2026-08-29

**Purpose:** PvP, and any fight where enemies stand in a group.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Thador | Wilder | 1 |
| Middle | Eironn | Wilder | 1 |
| Middle | Faramor | Wilder | 1 |
| Back | Solise | Wilder | 6 |
| Back | Aurora | Celestial | 2 |

**Artifact:** Confining Spell +6.

**Why:** Eironn's Ultimate drags every enemy within 2 tiles into one pile, freezes them 3s and cuts their Magic DEF by 40%. Faramor's circle then punishes the stack and blocks enemy healing. Four Wilders plus Aurora wildcarding = **+22%**.

**Blocked on ascension.** Eironn only fires his Ultimate at battle start from **Mythic+**. He is Epic. Until then the pull is not guaranteed to land first, and the comp is a worse version of itself. Copies are the unlock. See [../mechanics/recruitment.md](../mechanics/recruitment.md).

**Swap:** Arden for Faramor once Arden is above Elite. He charges his Ultimate off Eironn's hit and is the named payload for this pattern.

---

## Shemira scaling carry — `blocked`

**Purpose:** long campaign fights, on an account with no Exclusive Equipment.

Eironn, Bonnie, Daimon, Shemira, **Ulmus (not owned)**

**Why:** the named build for this pattern. Shemira snowballs, Daimon shields, Bonnie strips enemy Haste and ATK, Eironn groups them.

**Blocked on Ulmus.** He is A-Level, so he comes off the **All-Hero** wishlist, never an Epic letter.

### Thador variant — `superseded` 2026-08-29

The block is on the *named* build, not on the pattern. Substituting an owned tank makes it fieldable today:

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Thador | Wilder | 1 |
| Middle | Daimon | Graveborn | 3 |
| Middle | Shemira | Graveborn | 4 |
| Back | Bonnie | Graveborn | 7 |
| Back | Hugin | Lightbearer | 20 |

**Artifact:** Confining Spell +6. Faction bonus **+10%**, from 3 Graveborn.

**Why it was offered:** long AFK fights suit a scaling carry, and Hugin is the one Hand at 120 who buffs the carry's ATK and Haste directly. Eironn was left out because his pull only fires at battle start from Mythic+, which the account has not reached.

**Superseded by Lightbearer Resonance**, which the user adopted on 2026-08-29. That comp pays +22% against this one's +10%, and stacks two engines. This variant keeps a real tank and real shielding, so it stays on the record as the fallback if the running comp cannot hold its frontline.

---

## Snow Stomper Dream Realm — `proposed` 2026-08-29

**Purpose:** the Snow Stomper boss only. See [../mechanics/snow-stomper.md](../mechanics/snow-stomper.md).

| Role | Hero | Faction | Range |
| --- | --- | --- | --- |
| DPS carry | Galahad | Mauler | 10 |
| Debuffer | Kruger | Mauler | 1 |
| Healer | Smokey & Meerky | Mauler | 8 |
| Buffer | Hugin | Lightbearer | 20 |
| Flex | Taichi & Agumon | Dimensional | 7, then 1 |

**Artifact:** Starshard Spell +5. True damage ignores the boss's defence.

**Why:** fills the four roles the guides agree on. Galahad's Time Recast makes another hero fire again, which is the whole point of a single-target damage race. Kruger and Taichi & Agumon are the only two heroes this account owns that the Snow Stomper guides name. Three Maulers pay **+10%**.

**Known compromise:** the boss's frontal Frost cone punishes melee, and both Kruger and the digivolved Taichi & Agumon end up at range 1. They are in for their kits, not their positioning.

---

## Superseded

Kept in place above, not moved here, so each comp sits next to the one that replaced it.

- **Levelling default** — replaced by Lightbearer Resonance, 2026-08-29.
- **Shemira scaling carry, Thador variant** — replaced by Lightbearer Resonance, 2026-08-29.

## Onward

- Which heroes are owned and at what tier: [roster.md](roster.md)
- Why a comp is shaped this way: [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md)
- The order to build a new one in: [../mechanics/team-building.md](../mechanics/team-building.md)
- Rows and range: [../mechanics/formation.md](../mechanics/formation.md)
