# Index

Every file in this repo, and the questions it answers. Read the pointer, then read only the files whose trigger matches the question.

Each line is `path — what it holds — read it when`.

## Account

- [account/roster.md](account/roster.md) — every hero owned, with faction, class, damage type, ascension tier and EX level, grouped by faction, each linking to its kit file — read when the question names a hero, asks what is owned, or needs a team built.
- [account/teams.md](account/teams.md) — the current comp for each purpose, with formation, artifact, status and known weak points, plus the rules for replacing one — read when the question asks for a team, names a mode that needs one, or proposes changing a comp; write to it whenever a comp is recommended.
- [account/progression.md](account/progression.md) — Resonance Level, Hands of Resonance, total power, AFK stage, artifacts owned, mode unlocks, recruitment state (diamonds, tickets, pity counters, Stargaze target), and which progression track the account is on — read when the question needs hero levels, account power, what is unlocked, which artifact is available, or what summon currency and pity the account is sitting on.
- [account/equipment.md](account/equipment.md) — Class Equipment levels for all six classes, Exclusive Equipment owned, Magic Charm loadouts — read when the question is about gear, charms, or how strong a class actually is.
- `notes` — the user's raw inbox, unfiled — read only when filing a new account update. Never quote it as truth; the `account/` files supersede it.

## Mechanics

- [mechanics/team-building.md](mechanics/team-building.md) — the ordered method for building a five-hero comp, and the checks to run before handing one over — read whenever a team comp is asked for.
- [mechanics/team-archetypes.md](mechanics/team-archetypes.md) — the comp patterns a team is built on (nuke, scaling carry, boss amplify, Ultimate engine, summon stack, sustain, control), the engine behind each, a matchup table, and which owned heroes fill them — read when the question asks which heroes work together, why a hero is good in one fight and bad in another, or what to build toward next.
- [mechanics/factions.md](mechanics/factions.md) — the seven factions, the stat bonus at 3/4/5 same-faction heroes, the counter wheel and its +/-15% damage — read when picking a faction core or countering an enemy faction.
- [mechanics/formation.md](mechanics/formation.md) — which row each class stands in, how base range overrides the class label, and when to break the default — read when a comp needs placing on the grid.
- [mechanics/game-modes.md](mechanics/game-modes.md) — every mode, its unlock, and how its rules change team building — read when the question names a mode or an in-game event.
- [mechanics/solo-battles.md](mechanics/solo-battles.md) — the single-hero World Map and story encounters, why the faction bonus and every ally-facing skill pay nothing in them, and what to pick on instead — read when the question names a solo battle, a duel, or a fight that deploys one hero.
- [mechanics/arcane-labyrinth.md](mechanics/arcane-labyrinth.md) — the roguelike dungeon run: 10-hero bench, HP and Energy carried between floors, relics, crests, Pure Crystals, Deep Labyrinth, and what all that demands of a comp — read when the question names Arcane Labyrinth, a relic, a crest, Fitz's Store or the Mistal Berserker.
- [mechanics/legend-trial.md](mechanics/legend-trial.md) — the four faction towers, their weekday rotation, 90 floors each, and the faction lock that shuts out Celestial, Hypogean and Dimensional heroes — read when the question names Legend Trial, a Tower of Light / Will / Nature / Eternity, or asks for a mono-faction comp.
- [mechanics/honor-duel.md](mechanics/honor-duel.md) — the 9-win/3-loss run, the four starting Artifact+hero combos and the 60-vs-70 badge trade, the two-stage deploy, the Duel Store and how to build in the mode — read when the question names Honor Duel or Honour Duel.
- [mechanics/snow-stomper.md](mechanics/snow-stomper.md) — the Snow Stomper Dream Realm boss, its six skills, the four team roles it demands and the artifact to bring — read when the question names Snow Stomper or asks for a Dream Realm team.
- [mechanics/seasons.md](mechanics/seasons.md) — permanent versus seasonal progression, what a season reset wipes, Season 7 Crown of Ashes, Soul Pact and Phantimals — read when the question touches a season, a Phantimal, or which track a mode belongs to.
- [mechanics/progression-systems.md](mechanics/progression-systems.md) — Resonating Hall, Resonance Level, Hands of Resonance, the free swap rule and the unverified level-swap reading, the ten ascension tiers and what each unlocks — read when the question is about levelling, ascending, who should hold a Hand of Resonance slot, or what a tier gives.
- [mechanics/equipment-and-charms.md](mechanics/equipment-and-charms.md) — Class Equipment, Exclusive Equipment, Magic Charms, per-class upgrade priority, how the class Level is derived from the six slots, and the disputed gear-versus-Resonance-Level rule — read when the question is about gear, EX weapons, or charm sets.
- [mechanics/artifacts.md](mechanics/artifacts.md) — what each permanent artifact does, its upgrade steps at +4/+8/+10, the permanent ranking and the Season 7 set — read when a comp needs an artifact picked, or when the question asks what an artifact does or whether upgrading it is worth it.
- [mechanics/diamonds.md](mechanics/diamonds.md) — every diamond sink with its price and cap, the spend order, and what never to buy with diamonds — read when the question is about diamonds, the Guild Store, the Emporium, buying Invite Letters or Stellar Crystals, Arena tickets, or whether to save or spend.
- [mechanics/recruitment.md](mechanics/recruitment.md) — the four summon banners, their currencies, rates and pity counts, the two wishlists including the five heroes picked for the Epic slots, and Stargaze Station with its target priority — read when the question is about summoning, pulling, diamonds, Invite Letters, a rate-up banner, a wishlist slot, or which Celestial or Hypogean to chase.
- [mechanics/diamonds.md](mechanics/diamonds.md) — every diamond sink with its price and cap, the spend order, and what never to buy — read when the question is about diamonds, the Guild Store, Stellar Crystals, Arena tickets, Quick AFK, or whether to spend or bank.
- [mechanics/heroes/README.md](mechanics/heroes/README.md) — a table of all 40 heroes owned, pointing at one file each holding that hero's kit, range and best use — read whenever a comp turns on what a hero actually does, then open only the heroes named.

## Root

- [RAG-ALTERNATIVE.md](RAG-ALTERNATIVE.md) — what retrieval pattern this repo uses instead of a vector database, its pros and cons, and where each part of it lives here — read when the question is about how this repo works rather than about the game.

## Keeping this file honest

A file that is not listed here, or in a second-hop index this file names, is invisible. Whenever a file under `account/` or `mechanics/` is created, renamed, or changes what it covers, edit its line here in the same turn. Run the `audit` skill to catch drift.
