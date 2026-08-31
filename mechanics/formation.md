# Formation and range

> **Covers:** where to stand heroes on the grid, how base range decides the row, and how many entities each hero actually puts on it.
> **Updated:** 2026-08-31

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

- **Taichi & Agumon** starts at range 7, then digivolves to WarGreymon at range 1. It opens as a backline attacker and ends as the frontline. **Start it in the back row, not the front.** Confirmed from the account: fielded in the front row it was killed before the digivolve landed. The +100% HP that makes it a frontliner arrives with the transformation, so the pre-digivolve form is a fragile range-7 attacker with a tank's job and none of a tank's HP. Once it transforms it walks to the front on its own.
- **Shadewing** is a Graveborn Rogue at range 1 doing magic damage. It has to reach the enemy to work.

## Count the entities, not the heroes

**A five-hero comp is rarely five tiles.** Some heroes put a second body on the grid, and one puts none of the two names on it. A formation that lists five heroes and five rows has not finished the job.

So every comp states, per hero, **how many entities it fields and where each one goes**. Say it hero by hero, because the count is a property of the hero, not of the comp.

Three kinds, and only the first is a placement the user makes.

### Placed at deploy

These take more than one tile before the fight starts, and each tile is a real choice.

| Hero | Entities | The rule |
| --- | --- | --- |
| Elijah & Lailah | 2: a **Melee Twin** and a **Ranged Twin** | Ranged Twin to the back row, Melee Twin to the middle, never the front. They **share one HP and Energy pool** carrying +50% max HP, so a hit on the forward body drains the bar the back one dies from. Blind pulses 1 tile around the Ranged Twin, Knockback around the Melee Twin. See [heroes/elijah-lailah.md](heroes/elijah-lailah.md) |
| Phraesto | 2: his **true body** and an **Illusion** | The Illusion is summoned in the preparation phase, so it stands before the first hit. **Both in the same row**, which is what grants each of them 30% damage reduction. Allies behind the Illusion take less damage; allies behind the true body gain Energy Recovery Speed, so the two bodies aim two different buffs. See [heroes/phraesto.md](heroes/phraesto.md) |

`?` whether the game sets the second tile itself or lets the user place each entity. The rows above are what to aim for either way.

### Fewer tiles than the name suggests

A paired name is not two bodies. Do not hold a tile open for the partner.

| Hero | Entities | Why |
| --- | --- | --- |
| Taichi & Agumon | 1: **Agumon** | Taichi stands **off the field, invincible**, and cheers Energy in from there. See [heroes/taichi-agumon.md](heroes/taichi-agumon.md) |
| Yamato & Gabumon | 1: **Gabumon** `?` | Yamato cheers the same way Taichi does, and no source states he is placed. Treat it as one tile until the account says otherwise. See [heroes/yamato-gabumon.md](heroes/yamato-gabumon.md) |
| Smokey & Meerky | 1 | One unit at range 8. The 2-tile aroma is drawn around that tile, so the comp is built inward around it. See [heroes/smokey-meerky.md](heroes/smokey-meerky.md) |

### Arriving during the fight

Not placed, but position still decides what they are worth, so a comp says where they land.

| Hero | What arrives | Where it matters |
| --- | --- | --- |
| Rolan | a **clone** on every ally Ultimate | it inherits 80% of the caster's base stats, so it follows whichever hero cast |
| Shemira | 10 **ghosts** per Ultimate, plus more when allies take heavy damage | they feed any summon buff on the team |
| Aurora | **Sonny** the unicorn, then **bunnies** | her own Hero Focus counts summons from **different** allies, so spread the sources |
| Zanie | 2 laser **turrets**, plus a gun turret | static, so her own tile decides their firing arc |
| Silven | 6 flying **blades** | launched off her normal attacks |
| Cecia | **Mr. Carlyle**, who inherits her stats | he hits in an arc |
| Chippy | **hamsters** he rides on | |
| Temesia | her **mount** | it leaps forward and knocks down |
| Velara | 4 **magic circles** | they heal allies, so they want the team inside them |
| Solise | **Bulbsprites** grown from bulbs handed to allies | the bulbs land on allies, so the sprites appear where the team stands |
| Kordan | the **Dominance Ring** | it buffs allies standing inside, so it is a zone to stand in |
| Faramor | a **magic circle** of true damage | a zone to put enemies in |
| Galahad | a **Magic Circle centred on her** | so her tile draws it |

## When to break the default

The three-row default is a starting point, not a rule.

- Enemy tanks stronger than yours: move your damage dealers up beside your tanks, so the fight happens where you choose.
- A Support with a short buff range: put it in front of the heroes it buffs, not behind them.
- A carry the enemy will dive: put a Tank on the tile between it and the enemy backline.

Check the range **and the entity count** of every hero in the comp before fixing the formation. See [heroes/README.md](heroes/README.md).

## Sources

- https://gamerant.com/afk-journey-best-team-comp-guide/
- https://molanaacademy.com/afk-journey-best-heroes-guide-and-powerful-formations/
- https://sportskeeda.com/esports/afk-journey-team-building-guide-best-team-compositions
