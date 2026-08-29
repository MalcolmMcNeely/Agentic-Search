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
5. **State the comp in the present tense.** No date on the heading, no note about what it replaced. Git holds that.

## Status

| Status | Meaning |
| --- | --- |
| `running` | the user fields this in game |
| `proposed` | recommended here, not yet confirmed in game |
| `blocked` | a hero is missing |

---

## AFK Stages, main — Lightbearer Resonance — `running`

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

**Two weak points:**

1. **One payload, four engines.** [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md) calls Rolan and Aurora engines, not carries. Hugin is support, Temesia is a tank. **Zanie** is the only real damage dealer.
2. **No healer.** Hugin gives cogshields and damage reduction. Rolan heals only as Morale climbs. Nothing heals on demand.

**Risk:** Aurora is an engine at range 2, so she has to come forward. Confining Spell is picked to keep enemies off her.

**First swap to try if it stalls:** Temesia out, **Solise** in, for healing and a team damage buff. It drops the core to 2 Lightbearer, so the bonus falls to +14%, and it leaves no tank. Test it, do not assume it.

**Open test:** Starshard fires every 4 ally Ultimates, and Rolan's clones cast Ultimates. If clones feed the counter, Starshard may beat Confining here. Unknown.

---

## AFK Stages, backup — Shemira scaling carry — `running`

**Purpose:** the saved second formation, for fights where the main comp's frontline collapses.

| Row | Hero | Faction | Range |
| --- | --- | --- | --- |
| Front | Thador | Wilder | 1 |
| Middle | Daimon | Graveborn | 3 |
| Middle | Shemira | Graveborn | 4 |
| Back | Bonnie | Graveborn | 7 |
| Back | Hugin | Lightbearer | 20 |

**Artifact:** Confining Spell +6. Faction bonus **+10%**, from 3 Graveborn.

**Why:** long AFK fights suit a scaling carry. Shemira snowballs and heals off her own ghosts, Daimon shields, Bonnie strips enemy Haste and ATK, Thador tanks and heals. Hugin buffs the carry's ATK and Haste directly. This comp has a real tank *and* real shielding, which the main comp does not.

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

## Dream Realm, Snow Stomper — `proposed`

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

## Arcane Labyrinth — Wilder sustain — `proposed`

**Purpose:** the Arcane Labyrinth run. Read [../mechanics/arcane-labyrinth.md](../mechanics/arcane-labyrinth.md) first: HP and Energy carry between floors, so this comp is built to end each fight healthy, not to end it fast.

**The five fielded:**

| Row | Hero | Faction | Class | Range | Tier |
| --- | --- | --- | --- | --- | --- |
| Front | Thador | Wilder | Tank | 1 | Legendary |
| Middle | Faramor | Wilder | Rogue | 1 | Legendary |
| Middle | Aurora | Celestial | Mage | 2 | Legendary |
| Back | Hewynn | Wilder | Support | 4 | Epic |
| Back | Solise | Wilder | Support | 6 | Legendary |

**The bench, slots 6 to 10.** This mode picks 10 heroes, not 5. Spend these on early floors and keep the five above fresh.

| Hero | Faction | Class | Tier | Why |
| --- | --- | --- | --- | --- |
| Velara | Wilder | Support | Epic | third healer, keeps the Wilder core if she subs in |
| Smokey & Meerky | Mauler | Support | Epic | sustained healing plus an ally ATK buff |
| Antandra | Mauler | Tank | Epic | replacement frontline: taunt, 60% damage cut, self-heal |
| Lily May | Wilder | Rogue | Epic | replacement damage, keeps the Wilder core |
| Hugin | Lightbearer | Support | Legendary | cogshields and an ATK buff |

**Artifact:** Awakening Spell +6. [../mechanics/artifacts.md](../mechanics/artifacts.md) names it for this mode, and the reason is the carryover: heal that is wasted in a normal fight is banked here.

**Faction bonus: +22%.** Four Wilder plus Aurora wildcarding, plus +1% ATK and HP for the Celestial.

**Why:** the mode is attrition, so the comp is **sustain with offence** from [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md), not nuke. Hewynn is the account's best dedicated healer and also strips debuffs and cuts team damage taken. Solise heals in waves and her Bulbsprites raise team damage, so the second healing slot still adds damage. Thador tanks and his Ultimate heals the team on top. Faramor is the payload: true damage, blocked enemy healing, and a 12 to 15% ATK buff on the ally beside him. Aurora raises the damage of every allied summon, which pays Solise's Bulbsprites and her own, and turns nearby enemies into immobilised plushies.

**Relic plan:** stack one type for the crest at 2, 4, 6 and 8. Warmth, Fortitude or Guard. Do not spread across all four slots.

**Four weak points:**

1. **No Hand of Resonance is in the fielded five.** That costs nothing while every hero sits at the Resonance Level, and starts costing as soon as a Hand is levelled past it. Move Hands onto Hewynn, Solise, Faramor and Thador. See [../mechanics/progression-systems.md](../mechanics/progression-systems.md) and [progression.md](progression.md).
2. **Faramor is the only real damage dealer.** Aurora and Solise add summon damage, but a floor with a hard timer or a high-HP boss can stall.
3. **Thador and Faramor are both range 1**, so both walk into the enemy and leave Aurora at range 2 exposed once the front moves up. Watch her HP, because it carries.
4. **Healer role split is `unverified`.** gamerant says bring two healers, afk.guide says one is enough. This comp follows gamerant, which costs a damage slot. See [../mechanics/arcane-labyrinth.md](../mechanics/arcane-labyrinth.md).

**First swap to try if runs stall on damage:** Aurora out, **Cecia** in. She steals 1.5% of the target's two DEF stats every second and keeps it for the fight, and Mr. Carlyle can be resummoned to heal. It drops the bonus from +22% to +18%.

**Open question for the user:** [progression.md](progression.md) records Arcane Labyrinth progress as `?`. Which difficulty and floor is the account on now?

---

## Legend Trial, Tower of Nature — Wilder sustain — `running`

**Purpose:** Tower of Nature only. Faction-locked to Wilder. Open Wednesday, Saturday, Sunday. **Floor 37 of 90**. See [../mechanics/legend-trial.md](../mechanics/legend-trial.md).

| Row | Hero | Class | Range | Tier |
| --- | --- | --- | --- | --- |
| Front | Thador | Tank | 1 | Legendary |
| Middle | Faramor | Rogue | 1 | Legendary |
| Middle | Eironn | Rogue | 1 | Epic |
| Back | Hewynn | Support | 4 | Epic |
| Back | Solise | Support | 6 | Legendary |

**Artifact:** Awakening Spell +6. [../mechanics/legend-trial.md](../mechanics/legend-trial.md) names it for this mode on a healer team, and this is one.

**Faction bonus: +22%.** Five Wilder is forced by the lock, so the cap is free.

**Why:** 90 floors of rising enemy stats is attrition, so this is **sustain with offence** from [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md). Faramor is the payload: true damage, blocked enemy healing, damage scaling off HP the enemy has already lost, and a 12 to 15% ATK buff on the ally next to him. Thador tanks and his Ultimate heals. Hewynn is the account's best healer and strips debuffs. Solise heals in waves and her Bulbsprites raise team damage, so the second heal slot still adds damage. Eironn bunches the enemy and cuts Magic DEF by 40%.

**Aurora and Rolan are locked out.** Celestials do not wildcard inside a tower. Confirmed from the account, see [../mechanics/legend-trial.md](../mechanics/legend-trial.md).

**Three weak points:**

1. **No Hand of Resonance is in these five.** That costs nothing while every hero sits at the Resonance Level, and starts costing as soon as a Hand is levelled past it. Move Hands onto Faramor, Thador, Hewynn and Solise. See [../mechanics/progression-systems.md](../mechanics/progression-systems.md).
2. **Eironn is Epic, so his battle-start pull does not fire.** That needs Mythic+. He is in for the Magic DEF cut and the mid-fight bunching, not the opening nuke.
3. **Faramor is the only real damage dealer.** A floor with a high-HP wall can stall.

**First swap to try if floors stall on damage:** Eironn out, **Arden** in, for AoE and crowd control. Arden is Elite, two tiers under Eironn, so he dies fast on high floors. Test it, do not assume it.

**Left home on purpose:** Lily May, an S+ **PvP** counter-pick with no job in PvE. Velara, outclassed by Hewynn as the healer. Lenya, an isolate-and-duel kit at Elite+.

---

## Legend Trial, Tower of Eternity — Graveborn scaling carry — `running`

**Purpose:** Tower of Eternity only. Faction-locked to Graveborn. Open Thursday, Saturday, Sunday. **Floor 36 of 90**. See [../mechanics/legend-trial.md](../mechanics/legend-trial.md).

| Row | Hero | Class | Range | Tier |
| --- | --- | --- | --- | --- |
| Front | Valka | Warrior | 1 | Epic+ |
| Middle | Daimon | Warrior | 3 | Legendary |
| Middle | Shemira | Mage | 4 | Legendary |
| Back | Cecia | Marksman | 5 | Epic |
| Back | Bonnie | Marksman | 7 | Legendary |

**Artifact:** Confining Spell +6. The frontline here is one Warrior, so keeping 2 enemies out of the backline matters more than the healing Awakening would add.

**Faction bonus: +22%.** Five Graveborn is forced by the lock.

**Why:** this is the **scaling carry** pattern from [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md), which suits long floor fights. Shemira is the carry: her ghosts snowball, heal her, and can be spent for true damage off enemy max HP. Daimon shields the team and soaks. Bonnie's Aging strips enemy Haste and ATK, then spreads it. Cecia is the second damage dealer, and her Trial of Thorns steals 1.5% of both enemy DEF stats every second and keeps it for the whole fight, which compounds the longer a floor runs. Valka holds the front and shields nearby allies.

**Only 6 Graveborn are owned, so this comp is 5 of 6.** Shadewing is the one cut: Elite tier, range 1, and pure single-target damage the comp already has.

**Three weak points:**

1. **There is no Tank.** Valka is a Warrior standing in for one, and her file marks her weak in ordinary campaign content. This is the comp's real ceiling.
2. **There is no healer.** Shemira heals only herself, off her own ghosts. Daimon's shields are the whole defence.
3. **No depth behind it.** A wall on this tower cannot be answered by swapping a hero in, only by ascending the six that exist.

**Daimon is a Hand of Resonance**, so levelling him is one fifth of raising the Resonance Level. See [progression.md](progression.md).

---

## Purposes with no comp yet

Battle Drills, Supreme Arena, and the two Legend Trial towers this account cannot fill yet: **Tower of Light** (Lightbearer, 12 owned) and **Tower of Will** (Mauler, 8 owned). Both have the roster depth, neither has a comp written. See [../mechanics/legend-trial.md](../mechanics/legend-trial.md).

## Onward

- Which heroes are owned and at what tier: [roster.md](roster.md)
- Why a comp is shaped this way: [../mechanics/team-archetypes.md](../mechanics/team-archetypes.md)
- The order to build a new one in: [../mechanics/team-building.md](../mechanics/team-building.md)
- Rows and range: [../mechanics/formation.md](../mechanics/formation.md)
