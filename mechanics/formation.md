# Formation and range

> **Covers:** where to stand heroes on the grid, how base range decides the row, how many entities each hero actually puts on it, and every kit that reads a tile rather than a row.
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

**Each body gets its own tile, and the user places every one.** Confirmed from the account: Phraesto takes one tile for himself and a second for his Illusion. So a comp holding both heroes above is **seven** placements, not five.

**Placing a hero can draw a marker on another tile, and the marker is part of the placement.** Confirmed from the account for Phraesto: a marker appears on a tile decided by where he is put. Read it before locking the formation, because it shows where the second body lands.

### Fewer tiles than the name suggests

A paired name is not two bodies. Do not hold a tile open for the partner.

| Hero | Entities | Why |
| --- | --- | --- |
| Taichi & Agumon | 1: **Agumon** | Taichi stands **off the field, invincible**, and cheers Energy in from there. See [heroes/taichi-agumon.md](heroes/taichi-agumon.md) |
| Yamato & Gabumon | 1: **Gabumon** | Yamato stands **off the field** and cheers from there, the same shape as Taichi. Confirmed from the account. See [heroes/yamato-gabumon.md](heroes/yamato-gabumon.md) |
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

## Placement-relative skills, and the markers that show them

Some skills do not read a row. They read **which tile a hero was put on, relative to another tile**, and they lock that reading in during the preparation phase, before the first hit. A comp that names rows and stops has not set these.

**The game draws a marker for them.** Confirmed from the account: placing Phraesto puts a marker on a second tile, chosen by where he was put. Read the marker before locking the formation. `?` whether every hero below draws one, and whether a marker tile can be dragged on its own. No guide covers the marker UI; this is an account fact with no source behind it.

Every owned hero whose kit reads position:

| Hero | What it reads | What to do |
| --- | --- | --- |
| Elijah & Lailah | **Stellar Bond draws a straight line between the two twins when they are aligned.** Allies standing **between** them on that line are linked | see the trade below. Aligning them across an ally is a decision, not a default |
| Phraesto | which body an ally stands **behind**: the Illusion gives damage reduction, the true body gives Energy Recovery Speed. Both bodies in **one row** gives each 30% damage reduction | two rules at once, and they can conflict. Row first, then aim each body at the ally that wants its buff |
| Thador | **the ally placed 1 tile behind him becomes his lieutenant**, fixed during preparation | put the hero that most needs a shield on that tile. It absorbs 350% + 35% for 8s, rising to 380% + 35% at level 191 |
| Taichi & Agumon | at battle start WarGreymon buffs **himself and every ally behind him** with +25% of his own ATK for 20s | stand the allies you want buffed behind him, not level with him |
| Yamato & Gabumon | Grace Cross Freezer **fires more missiles the closer allies stand** | bunch the team, do not spread it |
| Smokey & Meerky | the aroma is **2 tiles wide** around their own tile, and 3 allies inside it turn on the Hero Focus clause | build the comp inward around their tile |
| Faramor | Sacred Pledge buffs him and **one adjacent ally** | put a damage dealer on a neighbouring tile |
| Kordan | the Dominance Ring buffs allies **standing inside it** | it lands on the target, so it pulls allies forward |
| Rowan | his Ultimate grants Energy to allies **within 2 tiles**, after he moves up to one tile | keep him inside 2 tiles of the heroes whose Ultimates matter |
| Hugin | he **anchors himself to the anvil tile** and buffs and shields nearby allies | his tile is fixed once cast, so pick it for the allies, not for him |

### The Elijah & Lailah trade

Linking allies is not free, and on this account it is a real choice rather than an obvious gain.

**Linked allies get:** Lailah's green glow heals each of them along the path for 100% + 10%, and Elijah's golden glow restores their Energy. If every linked ally **excluding the twins** shares one faction, a resonance adds +10 Vitality and +10% Energy gained.

**The twins pay:** Stellar Bond grants them a permanent **+25% ATK while no other ally is linked**. `unverified`: one source says that bonus drops by 5% per linked ally, and no other source states the decrement.

`unverified`: the skill text says allies linked through Stellar Bond are **"unaffected during the dance"**, and no source says whether that excludes them from Starlight Waltz's +60 Haste or makes them immune to control while it runs. It is the difference between linking being a bonus and linking costing the comp its main buff. Settle it in game before building on it.

`unverified`: one pre-release source says the twins gain 5% ATK standing close together and 15% DEF standing far apart. Nothing since repeats it, and no dated in-window page confirms it.

**On this account the resonance cannot fire in the push comp**, which holds Graveborn, Dimensional, Hypogean and Celestial. So linking there buys the heal and the Energy only. See [../account/teams.md](../account/teams.md).

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
- https://www.prydwen.gg/afk-journey/characters/elijah-and-lailah (Stellar Bond draws a straight line between the aligned twins and links the allies between them; +25% ATK while nobody is linked; Lailah's glow heals linked allies 100% + 10%; the faction resonance; "unaffected during the dance". 402 on direct fetch, read through search summaries) [2026]
- https://www.prydwen.gg/afk-journey/characters/thador (the ally 1 tile behind Thador becomes his lieutenant during preparation; shield 350% + 35% for 8s, rising to 380% + 35% at level 191; guide dated 30 July 2026) [2026-07-30]
- https://afk-journey.fandom.com/wiki/Elijah_%26_Lailah (same Stellar Bond line mechanic, independently; linked allies gain ATK and both DEF stats worth 20% of the highest among other linked allies, capped at 40% of the twins' own. 402 on direct fetch, read through search summaries) [2026]
- https://lootbar.gg/blog/en/afk-journey-twins-leaked-strategic-tips-for-dominating-pvp.html (the only source for the 5% ATK close / 15% DEF far claim and for the 5%-per-link decrement; it is a **pre-release leak** article with no findable date, so both readings are carried as `unverified` and nothing newer repeats them) [undated, out of window]
