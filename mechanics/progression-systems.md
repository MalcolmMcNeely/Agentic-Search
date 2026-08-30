# Progression systems

> **Covers:** Resonating Hall, Resonance Level, Hands of Resonance and how to swap one, ascension tiers, and what each tier unlocks.
> **Updated:** 2026-08-30

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

**Why it matters.** The swap is free, so the five Hands should be the five heroes actually fielded, not whoever was levelled first. Only Hands get the +10. See [../account/progression.md](../account/progression.md) for who holds the slots now, and [team-building.md](team-building.md) for how the level gap feeds a comp.

Past Resonance Level 240, **Resonance Synergy** unlocks and takes Hero Essence.

## Ascension tiers

Ten tiers, in order:

```
Elite -> Elite+ -> Epic -> Epic+ -> Legendary -> Legendary+ -> Mythic -> Mythic+ -> Supreme -> Supreme+
```

A-Level heroes start at Elite. S-Level heroes start at Epic. Rare heroes (Hammie, Chippy) cannot ascend at all.

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
- https://afk-journey.fandom.com/wiki/Resonating_Hall (swap free and at any time, levels swap, resources returned; page returned 402 on direct fetch, read through search summaries)
- https://www.lootbar.com/blog/en/afk-journey-resonating-hall-guide-optimal-resonance-setup.html (swap free at any time; its claim that the incoming hero enters at the Resonance Level is contradicted by the account)
- https://www.afk.global/afk-journey-resonating-hall (swap at any time, subject to the level requirement; same contradicted claim as lootbar)
- https://levelpush.com/afk-journey/hero-ascension-tiers/
- https://playafkjourney.com/hero-ascension/
