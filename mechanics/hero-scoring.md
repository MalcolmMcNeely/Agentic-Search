# Hero scoring

> **Covers:** how to rank a hero from its kit alone, with no guide, and why a guide that never names a hero proves nothing about it.
> **Updated:** 2026-08-30

A fight is a race. Your five heroes deal damage until the enemy dies. The enemy deals damage until your five die. Whoever runs out of health first loses.

Every hero pays into one of two sums. The good ones pay into both.

- **Time alive.** The extra seconds the team survives.
- **Damage out.** The damage the team deals per second.

Score a hero on what its kit adds to those two sums. That is the method. It needs no guide and no tier letter, so it works the day a hero is released.

## Score the whole roster

Every hero the account owns is a candidate, and each one earns its place from its own kit.

A fan guide is an opinion with a date on it. The game patches, collab heroes arrive, and the guide stays where it was, so its hero list describes an earlier roster. Call that gap **guide silence**: the guide has nothing to say about a hero released after it was written.

Two rules follow.

- Score a hero the guides never name from its kit, at full weight, exactly like any other hero.
- Check a source's date, then read its rankings as evidence about the heroes it covers. See the recency check in the `game-research` skill.

The same holds for a hero the guides praise. Score it from its kit, because the guide may be ranking it for a mode this account is not playing.

## Tier gates

The mirror of guide silence, and the one that stings more. **A guide describes a hero at its ceiling.** The copy on the roster may be several ascensions below that, and a skill that is not unlocked pays nothing.

**Legendary+ unlocks Hero Focus, a permanent stat buff or passive effect. Mythic+ unlocks Exclusive Equipment and the new skill it carries.** So a hero below its breakpoint is a different hero. See [progression-systems.md](progression-systems.md).

Before crediting a hero with a skill, check two numbers: the tier the skill unlocks at, and the tier in [../account/roster.md](../account/roster.md).

**Galahad is the worked example.** Every team guide builds her boss amplify role on **Time Recast**, which fires another hero's Ultimate again. The guides are right that she has it. It unlocks at **Mythic+**, and she is **Legendary** on this account, with Legendary+, Mythic and Mythic+ all in between. So the comps naming her as an Ultimate-duplicator describe an account three ascensions from this one.

Guide silence undersells a hero on the roster. A tier gate oversells one. One move cures both: read the kit, then read the tier.

## What counts as time alive

Healing is one entry on a longer list. All of these buy seconds.

| Kit line | Why it buys time |
| --- | --- |
| Heals and rolling heals | direct |
| Shields and damage reduction | direct |
| Invincibility | direct, and no amount of enemy damage gets through it |
| Taunt | moves damage onto the hero built to eat it |
| Freeze, stun, sleep, knockback, flee | an enemy that cannot act deals zero damage |
| An enemy ATK cut | every point cut is damage you never take |
| Raw HP on a frontliner | direct |

**Control is survival.** A 5s freeze on the enemy carry deletes 5s of its damage. A heal does the same arithmetic, but control also stops burst, and a heal does not.

## What counts as damage out

ATK is one entry on a longer list here as well.

| Kit line | Why it adds damage |
| --- | --- |
| ATK and Crit buffs | direct |
| Haste and ATK SPD | more attacks in the same seconds |
| Energy handed to an ally | an Ultimate is most of a hero's damage, so Energy is damage |
| An extra cast, such as a clone or a recast | a whole extra Ultimate |
| An enemy DEF strip | your damage lands harder |
| Summons | extra bodies attacking |
| True damage | ignores enemy DEF, so it holds up against an armoured boss |

**Energy is damage.** This is the line that gets missed. A hero that gives no ATK at all, but doubles how often the carry fires its Ultimate, is a damage hero.

## Compare across the team, not per hero

The same buff is worth more when it lands on more heroes. Convert to a team total before comparing two heroes.

- +50% ATK on the carry beats +25% ATK on the carry.
- +25% ATK on four damage dealers beats +50% ATK on one.
- A team-wide 50% damage reduction is five heroes' worth of survival, bought with one slot.

## Ramp

Some kits pay nothing at battle start. They need stacks, a transformation, a kill, or an ascension tier before they switch on. That delay is the hero's **ramp**.

Ask two questions.

1. How many seconds until the kit switches on?
2. Does this fight last that long?

A long ramp costs nothing in AFK Stages, Dream Realm and Legend Trial, where fights run for minutes. It is fatal in Arena, where the fight is settled in the first ten seconds. One hero can be the best and the worst pick on the roster on this question alone.

Ramp is also why a feeder standing next to a ramp hero pays double. Anything that shortens the ramp multiplies the entire payoff behind it.

## What scoring cannot tell you

A kit description gives skill effects. It does not give base stats or scaling coefficients.

So scoring produces a **ranking**, not a simulation. It says hero A probably beats hero B in this fight. It does not say by how much. When two heroes score close, take the higher ascension tier, because a tier gates whole skills. See [progression-systems.md](progression-systems.md).

## Where this gets used

- [team-building.md](team-building.md) calls this at the carry and role steps.
- [team-archetypes.md](team-archetypes.md) places every owned hero into a pattern, and this is how a hero with no guide coverage earns its place there.

## Sources

This file holds method, not game facts, so it carries no external source. It is derived from the kits in [heroes/README.md](heroes/README.md) and the mode rules in [game-modes.md](game-modes.md).
