# Team building

> **Covers:** the factors that decide a good five-hero comp, and the order to apply them.
> **Updated:** 2026-08-29

A team is five heroes. Build it in this order.

A comp wins by dealing enough damage before it dies. So every slot is judged on two sums: the seconds it adds to the team's life, and the damage it adds per second. [hero-scoring.md](hero-scoring.md) holds the method for reading those two sums off a hero's kit, with no guide involved. Use it at steps 2 and 4, and use it on **every** owned hero, including the ones no guide has heard of.

## 1. Read the fight

What the enemy is decides everything downstream. Note the enemy faction, whether the damage is single-target or spread, and the mode's rules. See [game-modes.md](game-modes.md).

## 2. Pick the carry

One hero does most of the damage. Everything else exists to keep that hero alive, in range, and firing its Ultimate. Pick the carry before the faction core, never after.

Pick it by scoring kits, not by copying a guide's tier letter. A guide ranks the heroes that existed when it was written, so the newest heroes on the roster score zero there by default. See the guide silence rule in [hero-scoring.md](hero-scoring.md).

## 3. Build a 3-hero faction core

Three of one faction pays twice:

- **+10% ATK and HP** for the whole team, rising to +18% at four and +22% at five. See [factions.md](factions.md).
- **That faction's Phantimal unlocks** through Soul Pact. An extra body in the fight, with its own skills and a Spirit Mark buff. See [seasons.md](seasons.md).

The Phantimal is the bigger of the two, so a 3-core is close to mandatory in seasonal modes.

The core should be the faction that **counters the enemy faction**, for the extra +15% damage. Counter beats bonus when the two conflict.

**Strong heroes still beat the bonus.** A +10% stat buff loses to a hero two ascension tiers higher, or one holding an Exclusive Equipment. Take the bonus when it is free, drop it when it costs a good hero.

Celestial and Hypogean heroes count as any faction, so they fill slots 4 and 5 without breaking a 3-core.

## 4. Fill the roles

Six classes exist: **Tank**, **Warrior**, **Marksman**, **Mage**, **Rogue**, **Support**.

A working default is one Tank, one Support (heal), one carry, and two flex. The Tank holds the frontline so the backline survives long enough to charge Ultimates. The Support keeps the Tank up.

Drop the Tank only when the fight has no melee threat. Drop the healer only when the fight ends before sustain matters.

## 5. Check the hard limits

- **Which track is this?** Permanent modes read the permanent Resonance Level and Class Equipment. Seasonal modes read the Season Resonance Level, Season Equipment, Season Artifacts and Magic Charms. See [seasons.md](seasons.md).
- Every hero sits at the Resonance Level, except the five Hands of Resonance, which may run up to +10. See [progression-systems.md](progression-systems.md).
- **Ascension tier** gates skills. Legendary+ and Mythic+ each unlock a skill, and Mythic+ unlocks Exclusive Equipment. A hero below its skill breakpoint is a different hero.

## 6. Attach the kit

Four systems, each with its own scope. See [equipment-and-charms.md](equipment-and-charms.md) and [artifacts.md](artifacts.md).

| Kit | Scope |
| --- | --- |
| Class Equipment | per class, shared by every hero of that class |
| Exclusive Equipment | per hero, needs Mythic+ |
| Magic Charms | per hero, 3 slots, seasonal, and the right set changes by mode |
| Artifact | one per team |

## 7. Sanity test

Answer these before handing over a comp:

- Does the account actually own all five heroes, at the tiers assumed? Check [../account/roster.md](../account/roster.md).
- Does the faction core hold at 3 or more, so the Phantimal unlocks?
- Is there an answer to the enemy's main damage type?
- Does the carry survive to its first Ultimate?
- Is the artifact named, and does it suit the mode?
- Was every owned hero eligible for this fight actually considered, or only the ones a guide names? Check the comp against the full archetype lists in [team-archetypes.md](team-archetypes.md).
- Does any hero here have a **ramp**, and does this fight last long enough to pay it? See [hero-scoring.md](hero-scoring.md).

A draft that passes these goes to the reconcile step of the `team-comp` skill, which compares it with [../account/teams.md](../account/teams.md) and writes the result there.

## Which pattern, not just which heroes

Steps 2 and 3 above pick a carry and a faction core. They do not say what the five heroes are meant to *do* together. That is [team-archetypes.md](team-archetypes.md): the engine-and-payload patterns, and the matchup table for choosing between them.

## Sources

- https://www.prydwen.gg/afk-journey/guides/team-building-advanced (blocked at time of writing, re-check)
- https://www.allclash.com/best-teams-in-afk-journey-campaign-dream-realm-arena/
- https://playafkjourney.com/teams/

