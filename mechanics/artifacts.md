# Artifacts

> **Covers:** what an artifact is, what each permanent artifact does, which fight each one suits, and the Season 7 set.
> **Updated:** 2026-09-01

One artifact is equipped per team, not per hero, and it pays the team twice.

- A **stat line** every hero on the team receives, which climbs with the artifact's level. Each artifact grants a different pair or trio of stats, and Blazing's is the only one of the six that grants DEF Penetration.
- An **Assistance effect** that fires during the battle.

**The effect has exactly two upgrade steps, at +4 and +8.** Two independent sources list those two and no other.

**The "+10 step" the guides describe is the stat line at its ceiling, not a third ability.** Every figure quoted as a +10 effect is a row in the artifact's stat table: Enlightening's +7.2 ATK SPD and +11.4% HP, Blazing's +7.8 DEF Penetration and +13.8% to both DEF stats, Ironwall's +6 Haste and +9 Vitality, Starshard's +4.8 Haste and +10.2% HP. So a level past +8 buys stats, and the real question is whether those stats beat another artifact's +4 or +8. See [../account/progression.md](../account/progression.md).

`unverified`: **whether +10 buys anything over +9.** The stat tables list identical values at 9 and 10 on all six artifacts, and identical values at 4 and 5. One source, so it is a reading rather than a fact, and the upgrade screen in game settles it in one look.

## Permanent artifacts (Starter Story)

Six artifacts, permanently effective in every season. They unlock at Dreamdelve point thresholds — Awakening 35, Confining 120, Starshard 220, Enlightening 320, Blazing 420, Ironwall 520 — and all six are owned.

### There is no per-mode ranking to borrow, so this file carries no letter column

Checked against the source contract in [tier-list-sources.md](tier-list-sources.md). Nothing passes it.

- **The vetted current sources rank heroes, not artifacts.** allclash, afk.global and Pocket Tactics have no AFK Journey artifact ranking at all. The artifact pages on allclash and afk.global are AFK Arena, a different game.
- **The rankings that do exist are blended.** LootBar publishes one [2026-06-25], inside the window, but it is a single list with no mode attached to any letter, which fails the first test of the three-part rule. pcgamesn publishes one [2024-12-19], twenty months old and outside the window entirely. Prydwen's artifact guide blocks fetching and carries no findable date.
- **The two rankings that can be dated disagree at the bottom.** pcgamesn puts Ironwall at B and Blazing at C. LootBar reverses it, Ironwall C and Blazing D. Neither states what it ranks for, so there is nothing to arbitrate between them.

What replaces the letters is what the repo can defend: the effect, the stat line, the fight each artifact suits, and where the account fields it.

### Which fight each one suits

| Artifact | Stat line at max | The effect | The fight it suits |
| --- | --- | --- | --- |
| Starshard Spell | Haste, HP | true damage wave taking a cut of every enemy's **current HP**, every 3 or 4 ally Ultimates | long fights, many Ultimates, and enemy defence that has outrun the roster |
| Confining Spell | ATK, HP | imprisons the **2 rearmost enemies** every 10 or 12s | a stacked back row with no healer, and any fight the enemy's opening decides |
| Awakening Spell | ATK, Phys DEF, Magic DEF | rolling heal on the 3 or 4 weakest allies | a team that already heals, and any mode where HP carries between fights |
| Blazing Spell | **DEF Penetration**, Phys DEF, Magic DEF | fireball at the weakest enemy every 5s for a cut of Team ATK | a comp paying full price against enemy defence, especially physical melee |
| Enlightening Spell | ATK SPD, HP | ATK SPD and control immunity on the **single rearmost ally** | exactly one hero in the back row, and that hero fragile and ranged |
| Ironwall Spell | Haste, Vitality | both DEF stats, Energy on Hit and a rolling shield on the **frontmost ally** | a team whose front row is the thing that breaks |

The account's own levels and deployment are in [../account/progression.md](../account/progression.md), and the comp-by-comp picks are in [../account/teams.md](../account/teams.md).

**`disputed`: the guides rank Confining above Starshard. This account shows the reverse on an Ultimate-heavy comp with a level deficit.** Starshard beat Confining on the AFK Stages push comp, confirmed from the account, and the account wins per [../CLAUDE.md](../CLAUDE.md). The reason is scaling: Confining blocks 2 enemies, which is worth the same whatever the stage, while Starshard takes a cut of the target's **current HP** as true damage, which is worth more as enemy defence and HP climb. Two conditions decide it, so check them before copying the swap:

- **How many Ultimates the comp casts.** Starshard fires every 3 ally Ultimates at +8. A comp with an Ultimate cloner or a resetting carry comes round far faster than one without.
- **How far the roster sits below the stage.** True damage ignores defence, so the wider the level gap, the more Starshard pays and the less raw damage does. See [../account/progression.md](../account/progression.md).

Confining stays the pick where a comp genuinely needs its backline held, such as a squishy carry in short range of an enemy dive.

## What each one does

### Confining Spell

3s into the battle, and every **12s** after, deals magic damage equal to **25% of Team ATK** to the **2 rearmost enemies** and leaves them unable to move or act for **1.5s**. Stat line: ATK and HP.

| Upgrade | Effect |
| --- | --- |
| +4 | the imprison lasts 2.5s |
| +8 | the cooldown drops to 10s |

**The 2 rearmost enemies are usually the enemy carry and whatever feeds it**, so this is control aimed at the half of the enemy team that deals the damage. [hero-scoring.md](hero-scoring.md) counts control as survival: an enemy that cannot act deals nothing for those seconds, and unlike a heal it also stops burst.

**Nothing about it scales with the ladder.** Two enemies held for 2.5s is the same effect at stage 1142 as at stage 1, and the damage is read off your own Team ATK rather than the enemy's stats. That is the whole of the argument in the `disputed` note above, and it cuts the other way in a short fight, where a fixed opening effect is exactly what is wanted.

**On this account:** Confining sits at **+8**, so both effect steps are live: the imprison lasts 2.5s and the cooldown is 10s. No effect step remains. It is the pick on five comps in [../account/teams.md](../account/teams.md).

### Starshard Spell

Every **4** Ultimates cast by allies, a flame wave hits all enemies for true damage equal to **16% of each target's current HP**, capped at **60% of Team ATK**, and cuts their ATK SPD by **60 for 4s**. Stat line: Haste and HP.

| Upgrade | Effect |
| --- | --- |
| +4 | damage rises to 24% of current HP, cap rises to 90% of Team ATK |
| +8 | the wave triggers every 3 Ultimates instead of 4 |

**A cut of current HP is the one output an uncapped ladder cannot inflate away.** True damage ignores defence, and reading the enemy's own HP means the number grows as the enemy does. Everything else a comp does is priced against a defence stat that keeps climbing. See [game-modes.md](game-modes.md).

**Its rate is a comp property, not an artifact property.** The trigger counts ally Ultimates, so a comp with a cloner or a resetting carry fires the wave far more often than one without. Two heroes on the push comp cast as their own units, and whether those casts count is `unverified` in [../account/teams.md](../account/teams.md).

**On this account:** Starshard sits at **+10**, so both effect steps are live and the stat line is at its ceiling: the wave hits for 24% of current HP, fires every **3** Ultimates, and adds +4.8 Haste and +10.2% HP to the team. **It is finished.** It holds six comps, more than any other artifact owned.

### Enlightening Spell

At battle start it raises the ATK SPD of **one hero, the rearmost ally in the back row**, by **80 for 15s**, and gives that hero **control immunity** for as long as the buff runs. It does not stack with itself. A patch removed the original start-of-battle delay, so it fires immediately. Stat line: ATK SPD and HP.

| Upgrade | Effect |
| --- | --- |
| +4 | ATK SPD bonus rises to 100 |
| +8 | duration rises to 20s |

**It buffs one hero and you cannot choose which.** The game picks the rearmost. On a comp with three heroes in the back row, the buff may not land on the carry.

**Control immunity on the rearmost ally is the answer to an enemy Confining Spell.** Confining imprisons the 2 rearmost enemies, and from the other side of the board your rearmost hero is one of those two. So Enlightening blanks half of an enemy Confining for the first 15 to 20 seconds. It is a counter that cannot be aimed, because the game still picks which hero gets it, but in Arena, where the fight is settled early, 20s covers most of the battle.

**On this account:** Enlightening sits at **+10**, so both effect steps are live and the buff runs 20s at +100 ATK SPD. Every comp in [../account/teams.md](../account/teams.md) has two or three heroes in the back row except Battle Drills Team 5, which is the one place it aims correctly.

### Awakening Spell

**5s** after the battle starts it summons Radiant Life, which restores the **3 weakest allies** by **7% of their Max HP every 10s** for the rest of the battle. Stat line: ATK, Phys DEF and Magic DEF, reaching **+4.2% ATK and +26.4% to both DEF stats** at max, the largest passive defensive line of the six.

| Upgrade | Effect |
| --- | --- |
| +4 | healing rises to 10% of Max HP |
| +8 | the heal covers 4 allies instead of 3 |

**The heal is rolling and small, so it wants a long fight and a team already surviving.** A team that dies to burst is not saved by 10% every 10 seconds. A team that grinds is.

**In Arcane Labyrinth the healing compounds, because HP carries between floors.** Healing a normal fight would waste is banked there instead. It is also the pick on a Legend Trial healer team. See [arcane-labyrinth.md](arcane-labyrinth.md) and [legend-trial.md](legend-trial.md).

**On this account:** Awakening sits at **+7**, so only the +4 step is live: 10% of Max HP, still on 3 allies. It is the pick on four comps in [../account/teams.md](../account/teams.md).

### Blazing Spell

Shoots a fireball at the **weakest enemy** every **5s**, dealing magic damage equal to **20% of Team ATK**. Stat line: DEF Penetration, Phys DEF and Magic DEF, reaching **+7.8 Penetration and +13.8% to both DEF stats** at max.

| Upgrade | Effect |
| --- | --- |
| +4 | damage rises to 30% of Team ATK |
| +8 | adds extra damage equal to 4% of the target's lost HP, capped at 20% of Team ATK |

**The stat line is worth more than the fireball.** One fireball every 5s read off your own ATK is a fixed contribution. DEF Penetration discounts **every** attack the whole team makes, and no other artifact of the six grants any. That is the argument that holds Starshard, applied to the rest of the comp rather than to one wave.

**Its ceiling is lower than Starshard's for the same reason Confining's is.** Penetration is a flat figure and the enemy's defence is not, so Starshard's cut of current HP keeps pace with the ladder where a flat number does not.

**On this account:** Blazing sits at **+10**, so both effect steps are live and the stat line is at its ceiling.

### Ironwall Spell

Blesses the **frontmost allied hero** at battle start: **+15% Phys DEF and Magic DEF**, and **+20 Energy on Hit**, for the rest of the battle. At battle start and every **12s** after, that hero also gets a shield worth **20% of their max HP**, lasting **6s**. The blessing cannot be dispelled. Stat line: Haste and Vitality.

| Upgrade | Effect |
| --- | --- |
| +4 | defence bonus rises to 20% |
| +8 | on the blessed hero's death, the blessing moves to the frontmost surviving hero, once per battle |

**Energy on Hit is the half that gets missed.** A tank takes hits constantly, so +20 Energy on Hit brings its Ultimate round faster, and [hero-scoring.md](hero-scoring.md) counts Energy as damage. The rest is time alive bought for one hero.

**Everything it does lands on one slot**, which is why it loses to artifacts that pay the whole team. It wins where the front row is the thing that breaks: a low-tier team, or a team with no dupes on its tank.

**On this account:** Ironwall sits at **+4**, so the defence bonus is 20%. It takes no comp off another artifact, and its value here is arithmetic: [../account/teams.md](../account/teams.md) fields five Battle Drills teams at once and the account held exactly five artifacts, so this is the sixth. The sixth team is a weak one whose front row is exactly its problem, which is the fight this artifact is for. See [battle-drills.md](battle-drills.md).

## Season 7 artifacts

12 Legendary artifacts exclusive to Crown of Ashes, enhanceable to +30. They reset at season end, and the account is permanent-track only, so none is reachable. See [seasons.md](seasons.md) and [../account/progression.md](../account/progression.md).

Swiftheal, Breakthrough, Vine Snare, Sunlance, Wing Guard, Surging, Arc Burst, Vanguard, Windcall, Frontline, Magicsurge and Valorshield Spell.

- **Breakthrough Spell** and **Arc Burst Spell** unlock early from Story Quests.
- **Sunlance Spell** and **Magicsurge Spell** come from Season Milestones and are the endgame picks.

Their effects are not recorded, and there is no reason to record them until the account reaches Season access at Resonance Level 240.

## Sources

- https://afk-journey.fandom.com/wiki/Artifact (what an artifact is, the Starter Story six, the 12 Crown of Ashes names, the patch history) [current]
- https://afk-journey.fandom.com/wiki/Confining_Spell (effect, both upgrade steps, stat table, Dreamdelve unlock) [current]
- https://afk-journey.fandom.com/wiki/Starshard_Spell (the same fields) [current]
- https://afk-journey.fandom.com/wiki/Enlightening_Spell (the same fields) [current]
- https://afk-journey.fandom.com/wiki/Awakening_Spell (the same fields) [current]
- https://afk-journey.fandom.com/wiki/Blazing_Spell (the same fields) [current]
- https://afk-journey.fandom.com/wiki/Ironwall_Spell (the same fields) [current]
- https://www.lootbar.com/blog/en/afk-journey-artifacts-guide-tier-list.html (second source confirming all six effects and both upgrade steps, and the modes each artifact is used in) [2026-06-25]. **Use with care** per [tier-list-sources.md](tier-list-sources.md). Its tier letters are one blended list with no mode attached, so they are not cited here.
- https://www.pcgamesn.com/afk-journey/artifacts [2024-12-19]. **Outside the 12-month window and not cited.** Listed only as the second of the two rankings that disagree above.
- https://www.prydwen.gg/afk-journey/guides/artifacts [no findable date, 403 to every fetch]. **Not cited**, because it cannot be dated. Re-check in a browser.
