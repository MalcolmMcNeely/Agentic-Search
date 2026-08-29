# Formation and range

> **Covers:** where to stand heroes on the grid, and how base range decides the row.
> **Updated:** 2026-08-29

Picking five heroes is half the job. Where they stand is the other half.

## Rows

| Row | Who | Why |
| --- | --- | --- |
| Front | Tanks | they soak the hits and hold the enemy off the backline |
| Middle | Warriors, Rogues, Support | close enough to fight or buff, far enough to survive |
| Back | Mages, Marksmen | they need distance to keep firing |

## Range decides the row, not the class label

Every hero has a base range in tiles, recorded in its file under `mechanics/heroes/`. Range beats the class name when the two disagree.

- Range 1 is melee. It walks to the enemy whatever row it starts in.
- Range 2 to 5 is short. It needs the frontline to hold or it gets reached.
- Range 6 and up is long. It fires from the back row untouched.

Two heroes on this account break their class label:

- **Taichi & Agumon** starts at range 7, then digivolves to WarGreymon at range 1. It opens as a backline attacker and ends as the frontline. Place it expecting the melee form.
- **Shadewing** is a Graveborn Rogue at range 1 doing magic damage. It has to reach the enemy to work.

## When to break the default

The three-row default is a starting point, not a rule.

- Enemy tanks stronger than yours: move your damage dealers up beside your tanks, so the fight happens where you choose.
- A Support with a short buff range: put it in front of the heroes it buffs, not behind them.
- A carry the enemy will dive: put a Tank on the tile between it and the enemy backline.

Check the range of every hero in the comp before fixing the formation. See [heroes/README.md](heroes/README.md).

## Sources

- https://gamerant.com/afk-journey-best-team-comp-guide/
- https://molanaacademy.com/afk-journey-best-heroes-guide-and-powerful-formations/
- https://sportskeeda.com/esports/afk-journey-team-building-guide-best-team-compositions
