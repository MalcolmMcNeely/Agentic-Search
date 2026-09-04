# Progression systems

> **Covers:** Resonating Hall, Resonance Level, Hands of Resonance and how to swap one, Resonance Synergy past 240, ascension tiers, and what each tier unlocks.
> **Updated:** 2026-09-04

## Resonating Hall and Resonance Level

Hero levels are not per-hero. The Resonating Hall syncs the whole roster to one number.

- The five highest-level heroes are the **Hands of Resonance**.
- The **lowest** Hand sets the **Resonance Level**.
- Every other hero on the account sits at exactly the Resonance Level, for free.
- Only Hands can be levelled up. A Hand may run at most **+10** above the Resonance Level.

So the way to raise the whole account is to level all five Hands evenly. Dumping XP into one Hand raises nothing but that Hand's own cap headroom.

### Swapping a Hand

The five Hands are **not** a locked choice.

- A Hand can be swapped for any owned hero **at any time**, and it **costs nothing**.
- The incoming hero **inherits the outgoing Hand's level**. Put a hero sitting at the Resonance Level into a Hand slot 10 levels above it and the hero takes that level; the outgoing hero drops to the Resonance Level. The +10 investment moves with the slot, it is never lost.
- The only restriction is the level rule above: after the switch the five Hands must still sit within 10 levels of each other.

**Confirmed from the account.** Swapping Daimon out for Rolan put Rolan on Daimon's level, not on the Resonance Level. Two guides (lootbar, afk.global) read the incoming hero as entering at the Resonance Level instead. The game disagrees with them, so the account wins, per [../CLAUDE.md](../CLAUDE.md).

**A swap cannot move the Resonance Level on its own.** That number is set by the lowest Hand, and a swap only exchanges two heroes' levels. Raising it still takes levelling the lowest Hand.

### The Hands are a loadout, not a commitment

Because the level travels with the slot and the swap is free and unlimited, the five Hands can be re-picked for whatever is being played.

- Build the Hands around the comp that is being pushed, and move them when the push changes.
- A hero needed at +10 for one mode can be swapped in before that run and swapped back out after. The hero leaving keeps nothing, but it costs nothing to bring it back.
- Only the **lowest** Hand is worth spending levels on. Levels put into any other Hand buy nothing but that hero's own headroom.

`unverified`, one source only (Fandom): heroes above level 1 outside the Hands had their levels reset when the Resonating Hall arrived, and **all levelling resources were fully returned**.

**Why it matters.** The swap is free, so the five Hands should be the five heroes actually fielded, not whoever was levelled first. Only Hands get the +10, and only while the Resonance Level is under its 240 cap. Past that cap the gap closes for good, and Resonance Synergy below takes over. See [../account/progression.md](../account/progression.md) for who holds the slots now, and [team-building.md](team-building.md) for how a comp reads a level.

## Resonance Synergy

**Resonance Synergy is the progression track that replaces the Resonance Level.** It unlocks when all five Hands stand at 240, which is the Resonance Level cap. It sits in the Resonating Hall, under the Power figure at the top left.

**It lifts the whole roster at once, not the five Hands.** Every Synergy level is applied to every hero owned, so the +10 Hand headroom that shaped comps below 240 stops existing. There is nothing left to lend, and no hero is left behind.

**It takes Hero Essence and nothing else.** Levelling to 240 cost Gold, Training Manuals and Hero Essence together. Past 240 the Gold and the Manuals stop being asked for, and each Synergy level costs more Essence than the one before it.

**Training Manuals recycle into Hero Essence at 3000 to 1.** That turns a stockpile the account can no longer spend back into the one resource that still counts. Hero Essence also drops from the Exploration Journal in non-season areas.

### The cap, and where it stops paying

| Figure | Value |
| --- | --- |
| Base cap | **300**, which is 60 Synergy levels |
| Per Supreme+ hero owned | **+5** on that cap |
| Levels that pay stats | the first **+60**, so up to level 300 |
| Levels past +60 | **no combat effect.** They pay **Diamonds** instead |

**The cap and the useful range are two different numbers.** The first 60 levels buy stats the way a Resonance Level did. The levels a Supreme+ hero unlocks above 300 buy Diamonds, not power. So ascending a hero to Supreme+ to raise this cap is a Diamond decision, never a combat one.

`unverified`: whether the +60 stat window is fixed at 60 levels or climbs with the cap as Supreme+ heroes raise it. One source states the +60 line and no second source repeats it.

## Ascension tiers

Ten tiers, in order:

```
Elite -> Elite+ -> Epic -> Epic+ -> Legendary -> Legendary+ -> Mythic -> Mythic+ -> Supreme -> Supreme+
```

A-Level heroes start at Elite. S-Level heroes start at Epic. Rare heroes (Hammie, Chippy) cannot ascend at all.

Ascending costs Soul Sigils, and for an A-Level hero the cheapest source is the Dream Store rather than a banner. The per-tier sigil counts are in [dream-store.md](dream-store.md).

### What tiers unlock

| Tier | Unlocks |
| --- | --- |
| Legendary+ | **Hero Focus**: a permanent in-battle stat buff or passive effect, different for every hero |
| Mythic+ | **Exclusive Equipment** (the EX weapon), which brings a new skill that grows as the weapon is upgraded |
| Supreme+ | **Enhance Force**: strengthens one skill the hero already has |

Every hero starts with three skills: Ultimate, Skill 1, Skill 2.

**Only Mythic+ adds a skill.** Legendary+ and Supreme+ both change what the existing kit already does rather than adding to it. So read a hero's Hero Focus as part of its stat line, and its Enhance Force as a footnote on the skill it upgrades.

**Hero Focus has three levels, and ascending does not raise them.** They are bought with **Tidal Essence**, so a Legendary+ hero and a Mythic hero can sit on the same Hero Focus level. Check the level in game before crediting a hero with the higher numbers.

Two worked examples on this account, both in the hero files: [heroes/aurora.md](heroes/aurora.md) gains ATK that scales off allied summons, and [heroes/kruger.md](heroes/kruger.md) gains Ranged DEF and no damage at all.

### Paragon

Hidden until 25 heroes reach Supreme+. Then excess Soul Sigils push heroes to Paragon 1 through 4. Paragon unlocks no skills, only stats.

- Paragon 1: 25 heroes at Supreme+
- Paragon 2: 20 heroes at Paragon 1
- Paragon 3: 15 heroes at Paragon 2
- Paragon 4: 15 heroes at Paragon 3

## Sources

- https://afk-journey.fandom.com/wiki/Gameplay_Guide/Function/Resonance_Level
- https://www.lootbar.com/blog/en/afk-journey-resonating-hall-guide-optimal-resonance-setup.html (swap free at any time; its claim that the incoming hero enters at the Resonance Level is contradicted by the account)
- https://www.afk.global/afk-journey-resonating-hall (swap at any time, subject to the level requirement; same contradicted claim as lootbar)
- https://afk-journey.fandom.com/wiki/Resonating_Hall (swap free and at any time, levels swap, resources returned. Resonance Synergy: unlocks with five Hands at 240, Hero Essence only, applied to every hero, stats until +60 then Diamonds, Training Manuals recycle 3000:1; 402 on fetch, read through search summaries) [in window]
- https://www.gamewitted.com/afk-journey/resonance-synergy-guide-for-afk-journey (base cap 300, +5 per Supreme+ hero, cost rises each level)
- https://levelpush.com/afk-journey/hero-ascension-tiers/
- https://playafkjourney.com/hero-ascension/
