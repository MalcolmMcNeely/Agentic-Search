# PvP team building

> **Covers:** why the general team-building method gives wrong answers in PvP, the four rules that replace it, and how to build an Arena defence and an Arena attack separately.
> **Updated:** 2026-09-09

[team-building.md](team-building.md) builds a team to beat the game. PvP is a different problem, and three of that method's steps mislead here. This file replaces them. Everything it does not overrule still applies.

## The four things the general method gets wrong in PvP

### 1. "A comp wins by dealing enough damage before it dies" is only the attacker's job

In Arena the **defender wins the timeout**. A defence that kills nothing and survives the clock has won. So the defence is not a weaker attack team, it is a team built for a different victory condition, and scoring it on damage per second scores the wrong sum. See [arena.md](arena.md).

**Score a defence on seconds alone.** Score an attack on whether it kills **all five** inside the clock, because leaving one alive is a loss.

### 2. Investment does not travel into Arena, and ascension does

**Arena caps every hero at a baseline level of 151, plus about 10%.** Levels, Resonance Synergy, Class Equipment and total power are all deleted at the door. **Unlocked skills are not.** See [arena.md](arena.md).

So the usual reasoning, that a well-funded hero beats a better-designed one, inverts. What is left is ascension tier, kit, faction percentages and placement.

**This makes the tier gate the first check in PvP rather than the last.** A guide rates a hero at its ceiling. In every other mode a low-tier hero is a good hero missing a skill, and the account's levels partly cover the gap. In Arena nothing covers it. **An Epic hero carrying an S+ PvP letter is not an S+ hero, because the letter is for a version of it that has Hero Focus and an Exclusive Equipment and this one does not.** See [hero-scoring.md](hero-scoring.md) and [progression-systems.md](progression-systems.md).

**The faction bonus is the exception that keeps its full value.** +10% at three, +18% at four, +22% at five, and the counter wheel's +/-15%, are all percentages of the capped stats, so they pay in Arena exactly what they pay anywhere. Against a flattened stat line they are a larger share of the total than usual. Take the bonus. See [factions.md](factions.md).

### 3. There is no such thing as "the Arena comp"

The general method ends with one comp per purpose. Arena is a **counter-picking mode**: you see three opponents, refresh free five times a day, and read each defence formation before spending a ticket. Building one team for all of them throws that away.

**Tailor the attack to the defence in front of you, and re-scout every time.** Defences get edited, so a plan that worked last week is stale information.

### 4. A comp that loses to one enemy hero is answered by a counter, not by a bigger version of itself

When the account loses to a defence built on a hero, the reply is the hero that shuts that hero down. Fielding the same engine with more money spent on it cannot work in a mode where the money is capped away.

## Building the defence

One team, saved, and every attacker fights it on the map saved with it.

- **Two tanks in the front row, three sustain or control heroes behind.** This is the shape every current source names.
- **Take heroes whose skills are all unlocked.** Ascension is the only investment that survives, so a Mythic hero with a middling letter beats an Epic hero with a great one.
- **Cutting enemy Haste is the strongest defensive stat in the mode**, because it steals the attacker's clock directly. Slowing the attack is the same as shortening it.
- **A revive, a cheat-death or a self-heal is worth more than a burst skill**, because each one adds seconds and nothing here needs to kill.
- **Pick the map that punishes a melee carry**, and place behind its low walls. Ranged units shoot over a low wall and melee units have to walk around it. See [formation.md](formation.md).
- **Do not bunch behind one healer if the common attack is one wide Ultimate.** Sustain that is all in one blast radius is not sustain.

## Building the attack

Built fresh per target, from three or four shapes rather than one comp.

1. **Scout the defence.** Note its faction, its frontline, whether it has a healer, whether it has a shield, and where it is bunched.
2. **Pick the shape that answers it**, then place for the defender's map.
3. **Take the faction that counters theirs** where a shape allows it, for the +15%.

| What the defence shows | What to bring |
| --- | --- |
| Stall, heals, no burst | **Anti-heal and burst.** Kill faster than it repairs. A long ramp loses to the clock |
| A shield wall that eats the opening | **True damage and sustained hits.** A timed shield absorbs a burst and expires against a stream |
| A single carry that wipes the team | **Control aimed at that hero**, before its window. A taunt, a stun, a freeze or an imprison |
| Everything bunched for one healer | **Area damage.** One cast reaches the whole cluster |
| Thin front row, exposed backline | **A dive.** Reach the supports first and the frontline holds nothing up |

**Spend all ten tickets.** Wins elsewhere on the ladder outweigh an occasional loss, and refusing a fight costs the same points as losing one when the tickets expire unused.

## The order to build in

1. **Read the fight.** For defence that is the clock; for attack it is the scouted formation and the map.
2. **Filter the roster by ascension tier first.** Set aside every hero whose key skills are not unlocked, whatever its letter.
3. **Pick the shape**, from the defence rules or the attack table above.
4. **Fill it, taking the faction bonus where it is free.** Celestial and Hypogean heroes count as any faction, so they hold a 3-core together.
5. **Place for the map**, not for the rows in the abstract. See [formation.md](formation.md).
6. **Attach the artifact.** One per team, and the pick differs between attack and defence: a defence wants stats and mitigation, an attack wants an effect that lands inside the clock. See [artifacts.md](artifacts.md).

## Sanity test

- Is every hero here holding the skills its letter was awarded for? Check [../account/roster.md](../account/roster.md).
- If this is a defence, does it survive with nothing killed? If this is an attack, does it kill **all five**?
- Was the defence formation scouted this session, or remembered?
- Does the plan answer the enemy's actual win condition, or restate the account's own?
- Does the faction core hold at three or more?

## Which modes this file governs

| Mode | Governed here | Note |
| --- | --- | --- |
| [arena.md](arena.md) | **Yes, fully** | The 151 baseline and the defender's timeout both apply |
| [supreme-arena.md](supreme-arena.md) | Yes, plus its own rules | Season mode, three teams, no repeated hero or artifact |
| [savannah-cup.md](savannah-cup.md) | Partly | Progression is equalised outright and the roster is drafted, so only the shapes carry over |
| [honor-duel.md](honor-duel.md) | Partly | The mode hands out its own heroes, so nothing in `account/` applies. That file stands on its own |

## Sources

- https://www.lootbar.com/blog/en/afk-journey-arena-of-heroes-a-guide-to-climb-the-ranks-quickly.html [2026, the level baseline, scouting before attacking, spending every ticket, the carry-plus-tank-plus-control-plus-support shape, the stall and lockdown defence archetypes, and the energy-rush, dive and burst attack archetypes]
- https://dotgg.gg/afk-journey/arena-guide/ [2026, the defender winning the timeout, two tanks and three sustain as the defence shape, tailoring the attack per opponent, re-scouting before every attack; 403 on direct fetch, read through search summaries]
- https://afk-journey.fandom.com/wiki/Arena [current, the 151 baseline and that unlocked skills are unaffected; 402 on direct fetch, read through search summaries]
- https://www.allclash.com/best-supreme-arena-teams-in-afk-journey/ [2026-05-18, that in-game Magic Charm recommendations are tuned for PvE and are wrong for PvP]
