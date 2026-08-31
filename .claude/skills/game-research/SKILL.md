---
name: game-research
description: Research an AFK Journey game rule on the web and write it into ./mechanics. Fires on a gap, meaning a faction rule, hero kit, artifact, charm, game mode or event detail that an answer needs and ./mechanics does not hold.
---

# Game research

AFK Journey patches often, and the fan sites disagree with each other and go stale. A file in `./mechanics` is only worth writing if a future session can trust it without redoing the search, so every fact lands with a source and every disagreement stays visible.

## Steps

1. **Check what already exists.** Read [INDEX.md](../../../INDEX.md) and the `mechanics/` file its pointer names. Extending an existing file beats creating a second file on the same topic.

2. **Search.** Prydwen and the Fandom wiki are the best sources and both block fetching often; when they do, fall back on allclash, afk.global, Pocket Tactics and gamerant. Search results themselves carry usable summaries when a fetch fails.

   **For anything ranked — a tier letter, a "best hero" list, a priority order — read [tier-list-sources.md](../../../mechanics/tier-list-sources.md) first.** It names the sources that pass the checks below, the sources that are banned outright, and the two traps that survive a date check: several sites that are really one opinion, and top-up resellers that inflate whichever hero is newest. playafkjourney, zilliongamer and gameleap are on the banned list; do not cite their rankings.

3. **Date the source, and throw it out if it is over a year old.** Every guide is an opinion with a date on it, and the game patches past it. Find the page's date, or the newest hero, artifact or season it mentions, and treat that as its date.

   **A source dated more than 12 months before today is not evidence.** Do not cite it, do not build a claim on it, and do not carry its numbers into a file. Search again with a narrower query, or with a different site, until a source inside the window turns up.

   **A source with no findable date is treated as out of window** unless the newest hero, artifact or season it names puts it inside one.

   **The one exception, and it is narrow.** When no in-window source covers the fact at all, an older one may be used only if the claim is written down as `unverified`, the source's date is stated in the file, and the passage says plainly that nothing newer confirms it. A future session must be able to see it is standing on old ground.

   Two failures follow from a stale source, and the second is the quiet one:

   - A **number** may have been patched since. Between two in-window sources that disagree, mark it `unverified` and show both. Never prefer one on age alone inside the window.
   - A **hero it never mentions** sits outside the source's scope, because the hero arrived later. Score that hero from its kit with [hero-scoring.md](../../../mechanics/hero-scoring.md), and read the source as evidence about the heroes it does cover.

   Write the scope down. When a source predates the thing asked about, say so in the file, so the next reader sees a gap rather than a verdict.

   **A displayed date can be a lie.** Several sites auto-stamp today's date on 2024 content. Date the page by the roster it names, using the dating key in [tier-list-sources.md](../../../mechanics/tier-list-sources.md), and let that beat the stamp.

   **For a ranking, 12 months is the hard floor but 6 months is the target.** A tier list ages faster than a rule, because every new hero re-ranks the old ones. Between two lists inside the window, the newer one wins on rankings — which is the opposite of the rule for numbers below.

4. **Check what a ranking is FOR before writing it down.** A tier list built for AFK Stages and one built for Arena disagree by design: the first fight runs minutes and pays for crowd control, the second is over in seconds and pays for burst. Neither list is wrong, and copying a letter across that line is.

   **A tier letter enters a file only with all three of these, and never without the first:**

   - **The mode it ranks for**, in the source's own words. A blended, "overall" or "general" list fails this and is not citable as a letter. Its ordering can still hint at a hero worth scoring from its kit.
   - **The dated source URL**, so the letter can be retired when it ages out.
   - **The investment level the source assumes**, or a plain note that the source does not state one. A list rating at Mythic+ with Exclusive Equipment describes a ceiling; compare it against `account/roster.md`.

   Then write the mode into the sentence, not just into the source line. `Dream Realm, rated S+ [allclash, 2026-08-26, assumes Mythic+]` survives a future audit. `rated S+` does not.

5. **Cross-check every number.** Percentages, unlock thresholds and level caps need two independent sources that agree. One source only, or two that disagree, gets written down as `unverified` with both readings shown. Never average two conflicting numbers into one.

6. **Check the finding against the account.** Read the matching file in `account/`. A rule the account visibly breaks is a stale guide, not a discovery about the account. Write the rule down as `disputed`, state what the account shows, and say the account is right. Example already in the repo: guides claim gear cannot exceed the Resonance Level, and the account holds level 160 gear at Resonance Level 110.

7. **Write it.** One topic per file, in `mechanics/`. A single hero's kit goes in `mechanics/heroes/<name>.md`. Every file opens with:

   ```
   # Title

   > **Covers:** the questions this file answers.
   > **Updated:** YYYY-MM-DD
   ```

   and ends with a `## Sources` list of the URLs used. **Put each source's date in brackets after its URL**, so the next session can retire it when it ages out of the 12-month window.

8. **Link it in.** Add or refresh the file's line in [INDEX.md](../../../INDEX.md), in the form `path — what it holds — read it when`. Link the new file from any sibling that should send a reader to it.

9. **Place a new hero in an archetype.** Writing `mechanics/heroes/<name>.md` is only half the job. A hero named in no archetype never gets drafted into a comp. Score its kit with [hero-scoring.md](../../../mechanics/hero-scoring.md) and add it to the matching archetype in [team-archetypes.md](../../../mechanics/team-archetypes.md) in the same turn, or to that file's **Placed nowhere** list with the reason.

Done when the question that triggered the research is answerable from the new file alone, every source is dated inside the last 12 months or carries the narrow-exception marking from step 3, every ranking names the mode it ranks for and the investment it assumes, every number in it either carries a source or says `unverified` or `disputed`, every source's date has been checked against what it fails to mention, the finding has been checked against `account/`, INDEX.md names the file, and any new hero stands in an archetype.

## Scope

Research the gap, not the topic. A question about one boss does not need the whole Dream Realm written up. A file that grows past what any single question needs is harder to keep current.
