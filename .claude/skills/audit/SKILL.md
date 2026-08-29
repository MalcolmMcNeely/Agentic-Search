---
name: audit
description: Check every file in the repo is indexed, linked and internally consistent. Fires when the user asks for an audit or a consistency sweep, and after a session writes or renames several files under ./account or ./mechanics.
---

# Audit

File-based retrieval has one documented weak point: the index is maintained by hand, so it drifts. A file nothing points at is invisible, and a pointer to a moved file is a dead end. This skill is the sweep that catches both.

Run the checks with shell commands, not by reading files one at a time. Report every failure with its file path. Fix what is unambiguous; ask about the rest.

## 1. Reachability

Every file under `account/` and `mechanics/` must be named by [INDEX.md](../../../INDEX.md), or by a second-hop index that INDEX.md names, such as `mechanics/heroes/README.md`.

```bash
for f in $(find account mechanics -name '*.md'); do grep -qr "$(basename $f)" INDEX.md mechanics/heroes/README.md || echo "UNREACHABLE: $f"; done
```

## 2. Dead links

Every relative link must resolve, in INDEX.md and inside every file.

```bash
for f in $(find . -name '*.md' -not -path './.claude/*'); do d=$(dirname "$f"); grep -oE '\]\(([^)]*\.md)\)' "$f" | sed 's/](//;s/)//' | while read p; do [ -f "$d/$p" ] || echo "DEAD: $f -> $p"; done; done
```

## 3. File contract

Every file under `account/` and `mechanics/` opens with `> **Covers:**` and `> **Updated:**`. Every file under `mechanics/` ends with a `## Source` or `## Sources` list. Every file under `mechanics/heroes/` carries all five fields: Faction, Class, Damage, Range, Level.

## 4. Account consistency

Re-run the checks in the `account-update` skill: the Resonance Level equals the lowest Hand, no Hand exceeds it by more than 10, there are exactly five Hands, every Hand appears in `roster.md` at the same tier, faction depth counts match the rows, and each class gear average matches its six slot numbers.

## 5. Drift between account and mechanics

List every rule in `mechanics/` marked `disputed` or `unverified` and check it against the account again. A rule the account now settles gets rewritten. A rule the account now breaks gets marked.

## 6. Open unknowns

List every `?` left in `account/`, and every "not recorded" left in `mechanics/`. Report them as a short list of questions for the user rather than guessing.

Done when all six checks have run, every failure is either fixed or reported, and the open unknowns are put to the user as a list.
