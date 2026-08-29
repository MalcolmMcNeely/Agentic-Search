---
name: game-research
description: Research an AFK Journey game rule on the web and write it into ./mechanics. Fires on a gap, meaning a faction rule, hero kit, artifact, charm, game mode or event detail that an answer needs and ./mechanics does not hold.
---

# Game research

AFK Journey patches often, and the fan sites disagree with each other and go stale. A file in `./mechanics` is only worth writing if a future session can trust it without redoing the search, so every fact lands with a source and every disagreement stays visible.

## Steps

1. **Check what already exists.** Read [INDEX.md](../../../INDEX.md) and the `mechanics/` file its pointer names. Extending an existing file beats creating a second file on the same topic.

2. **Search.** Prydwen and the Fandom wiki are the best sources and both block fetching often; when they do, fall back on allclash, playafkjourney, afk.global, gameleap, gamerant and bluestacks. Search results themselves carry usable summaries when a fetch fails.

3. **Cross-check every number.** Percentages, unlock thresholds and level caps need two independent sources that agree. One source only, or two that disagree, gets written down as `unverified` with both readings shown. Never average two conflicting numbers into one.

4. **Check the finding against the account.** Read the matching file in `account/`. A rule the account visibly breaks is a stale guide, not a discovery about the account. Write the rule down as `disputed`, state what the account shows, and say the account is right. Example already in the repo: guides claim gear cannot exceed the Resonance Level, and the account holds level 160 gear at Resonance Level 110.

5. **Write it.** One topic per file, in `mechanics/`. A single hero's kit goes in `mechanics/heroes/<name>.md`. Every file opens with:

   ```
   # Title

   > **Covers:** the questions this file answers.
   > **Updated:** YYYY-MM-DD
   ```

   and ends with a `## Sources` list of the URLs used.

6. **Link it in.** Add or refresh the file's line in [INDEX.md](../../../INDEX.md), in the form `path — what it holds — read it when`. Link the new file from any sibling that should send a reader to it.

Done when the question that triggered the research is answerable from the new file alone, every number in it either carries a source or says `unverified` or `disputed`, the finding has been checked against `account/`, and INDEX.md names the file.

## Scope

Research the gap, not the topic. A question about one boss does not need the whole Dream Realm written up. A file that grows past what any single question needs is harder to keep current.
