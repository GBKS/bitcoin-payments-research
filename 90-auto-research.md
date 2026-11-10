# Auto-research

*Cross-cutting plan: where AI agents could do research work in this library, a one-page pilot to test it, and its results. First pilot run November 9, 2026. Last updated November 10, 2026.*

Auto-research works best when progress fits in one number and a cheap test can measure it: propose a change, measure it, keep it if it's better, repeat. Cryptanalysis is a good fit: in Yukon's [HashSmash](https://www.yukon.org/hashsmash) challenge, AI agents compete to find cheaper collision attacks on reduced-round hash functions, and each submission's cost is scored automatically. A research library is a poor fit for that loop as a whole, because its real output is judgment, and no test can score judgment. The layer underneath the judgment is different: claims, numbers, sources and labels can be checked. This page proposes letting agents work on that layer, while people keep the conclusions.

## What fits, and what doesn't

| Work | Fit | What makes it checkable |
| --- | --- | --- |
| **Checking claims** against their sources | Good | Each verdict comes with a quoted passage that can be checked mechanically |
| **Keeping numbers current** (market caps, endpoint counts, merchant counts, usage figures) | Good | Each figure has a source and a date; freshness is measurable |
| **Testing each thesis** by looking for the strongest counterevidence | Medium | No single number, but adversarial search counters the author's bias; a person judges the result |
| **Drafting quick scans** for areas not yet covered | Weak | Only the form can be checked (template followed, every claim sourced or labeled), not the substance |
| **Primary research** (interviews, co-design, following live orders) | Poor | Needs people, consent and trust. Agents can help prepare and analyze, not run it |

## The claims list

To give the loops something to measure, each page gets a list of its checkable claims, kept as data next to the page (for example `claims/14-dollars-and-bitcoin.yml`). The Markdown pages stay as they are.

**What counts as a claim:** a number, date, event or attribution that could turn out to be wrong. A sentence with three numbers becomes three claims. Interpretations ("where the goal is dollar income, stablecoins win") are left to thesis testing.

| Field | What it holds |
| --- | --- |
| `id` | Short and stable, for example `14-05` |
| `text` | The exact wording on the page; if the page changes and it no longer matches, the record is flagged |
| `kind` | Number, date, event, attribution, or absence ("hasn't announced") |
| `label` | The label currently on the page: none, *from memory*, *to verify* |
| `source` | Link to the source |
| `quote` | The passage in the source that supports or contradicts the claim, at most about 25 words |
| `status` | Verified, partly, contradicted, unsourced or unreachable |
| `checked` | When it was last checked, and whether by an agent or a person |
| `note` | What's off, a better source, or a suggested rewording |

**Checks that need no agent:** every `text` still matches its page; every `quote` appears on its source page when fetched again; every `status` agrees with the label on the page.

## The pilot: one page

**Page:** [Dollars and bitcoin](14-dollars-and-bitcoin.md). It's short and full of numbers, with about 15–20 checkable claims: the Artemis figures, Tether's freezes, USDT on Lightning, Ark Labs' seed round, Blink's Dollar Balance, two items marked *to verify* and one absence claim.

**Steps:**

1. **Extract.** An agent lists the page's claims as records, without checking them. The author compares the list with their own reading, to see whether it missed or wrongly split any.
2. **Check.** For each claim, an agent opens the source, finds the passage and gives a verdict with a quote. It may propose a source where none is linked. It may not add claims or edit the page, and it reports "unreachable" rather than guessing.
3. **Recheck.** A second agent, given only the claim and the source and not the first verdict, checks again. Disagreements go to a person.
4. **Audit.** The author reviews every verdict. This is the actual experiment.
5. **Edits.** For claims found partly true or contradicted, an agent drafts corrections as one pull request. The author merges what holds up.

**What to measure:**

| Measure | How |
| --- | --- |
| Extraction completeness | Claims found ÷ claims the author would list |
| Verdict accuracy | Verdicts the author agrees with ÷ all verdicts |
| Made-up quotes | Quotes not found on the source page, checked mechanically; the target is zero |
| Recheck value | Errors caught in step 3 ÷ errors found in step 4 |
| Author's time | Minutes spent reviewing, against doing the checks by hand |
| Unreachable sources | How often agents can't open a source |

**Deciding what comes next:**

- **About 90% agreement or more and no made-up quotes:** claims lists for every page, mechanical checks on every pull request, scheduled refreshes of numbers, and agents proposing changes as pull requests.
- **About 70–90%:** keep a person in the loop, improve the agent instructions, and try a second page.
- **Below that, or a made-up quote that the recheck missed:** stop. The hard part is the check, not the agent, and that's worth writing up too.

## Pilot results: Dollars and bitcoin

Run on November 9, 2026. One agent extracted the claims; two agents checked them independently; the author audited every verdict. The claims, verdicts and quotes are in [claims/14-dollars-and-bitcoin.yml](https://github.com/GBKS/bitcoin-payments-research/blob/main/claims/14-dollars-and-bitcoin.yml).

| Measure | Result |
| --- | --- |
| Extraction completeness | 25 of 27 claims (93%) on a list written before seeing the agent's. Both misses were deliberate exclusions the agent flagged. |
| Agreement between checkers | 26 of 29 verdicts identical; the 3 differences were labeling or access, not substance |
| Verdict accuracy | 29 of 29 (100%): the author agreed with every verdict |
| Made-up quotes | None. Of the quotes a script could fetch, all were found verbatim on the source page (22 of 26 for one checker, 23 of 27 for the other) |
| Unreachable sources | 4 quotes from one news site couldn't be checked by script, because the site blocks automated requests; another site blocked one checker entirely |
| Author's time | About 15 minutes to audit 29 claims. Time to check them by hand: not yet estimated |

**What it found:** three corrections ("merchants," not "one merchant," also wrong in [Landscape](02-landscape.md); a "no published volumes" claim that overstated its source; a wallet's stablecoin "plans" that had since launched), and sources for two claims that had been marked *to verify*.

**What it means:** the pilot met the bar set above (about 90% agreement and no made-up quotes), so the next step is the full loop: claims lists for more pages, mechanical checks on pull requests, and scheduled refreshes of numbers. Two lessons for that loop: sites that block scripts need a fallback (an archived copy, or a person), and claims about something *not* happening can only be marked "nothing found as of" a date.

## Contributing with your own agent

The [prompt in CONTRIBUTING.md](https://github.com/GBKS/bitcoin-payments-research/blob/main/CONTRIBUTING.md#contributing-with-an-agent) is the checking step of this loop, run by a contributor's own agent on one claim at a time: pick an open [issue labeled `to verify`](https://github.com/GBKS/bitcoin-payments-research/issues?q=is%3Aopen+label%3A%22to+verify%22), find and open the sources, quote them, and let a person review before anything is submitted.

## Risks

- **Gaming the number.** The cheapest way to reduce unverified claims is to delete or weaken hard ones. Count removed and weakened claims alongside verified ones.
- **Made-up sources.** Language models invent plausible citations. Requiring a quote and fetching the page again is the defense.
- **Privacy.** Agents that search widely find individuals and small community accounts. The privacy rule in [Method](01-method.md) has to be checked, not trusted.
- **One kind of source.** Agents return to whatever ranks well. Track how varied the sources are.
- **Copyright.** Quotes stay short.

## Decisions so far

1. **The first pilot ran locally,** and its results were published afterwards, with the page edits.
2. **Claims lists live in `claims/`,** visible on GitHub but not on the site. Moving them to `_data/claims/` would let the site show a verification status later.
3. **Agents ran steps 1–3 and the author step 4.** That remains the cheapest setup that can still be inspected.
