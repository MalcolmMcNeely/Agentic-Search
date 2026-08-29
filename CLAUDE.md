# afkjourney

Management of my AFK Journey account. Also a worked example of agentic search, the file-and-pointer retrieval pattern that replaces RAG. See [RAG-ALTERNATIVE.md](RAG-ALTERNATIVE.md).

## Start here

[INDEX.md](INDEX.md) lists every file and the questions it answers. Read it before answering anything about the game or the account, then follow only the pointers that match. The `lookup` skill runs this.

## Layout

- `account/` holds the current state of my account: heroes owned, ascension tiers, Resonance Level, gear, artifacts, mode progress.
- `mechanics/` holds how the game works: factions, team building, formation, game modes, seasons, progression, gear, artifacts, and one file per hero under `mechanics/heroes/`.
- `notes` is my inbox. I dump raw account information there. It is input, never a source of truth. File it into `account/` and leave it alone otherwise.

## Rules

- Facts about the game get a source URL. Facts about my account come from me.
- **My account beats the guides.** The fan sites go stale between patches. When a guide and the account disagree, the account is right, and the mechanics file gets a `disputed` note saying so.
- A number two sources disagree on is written down as `unverified`, showing both. Never split the difference.
- A file that INDEX.md does not name, directly or through a second-hop index, is invisible. Write the index line in the same turn as the file.
- Every hero file carries the same five fields in the same order, so grep finds sets across the folder.

## Skills

- `lookup` fires on any question. Reads the index, follows pointers, greps for sets.
- `account-update` fires when I report account news.
- `game-research` fires on a gap in `mechanics/`.
- `audit` sweeps for unreachable files, dead links, contract breaks and drift. I can type it, and Claude may run it unprompted after writing a batch of files.
