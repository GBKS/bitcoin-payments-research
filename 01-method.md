# Method

*How the research in this library is done and written up. Last updated November 8, 2026.*

## Principles

1. **One step at a time.** Each document gets full attention, and each step is reviewed before the next. Findings from one step shape the next.
2. **Evidence over opinion.** Calls for input mostly capture what people *say*. Weight what they *do* and *make*.
3. **Specific over generic.** A good finding names a community, a concrete pain, an existing workaround and evidence, like KDOL for fan-funded ads. "Freelancers need payments" isn't a finding.
4. **Label what isn't verified.** Every claim is either linked to a source that was opened, or marked (see Evidence labels).
5. **Look beyond the respectable.** Bitcoin's real use has often been where banks won't go. Study those places too, and decide separately what any product builds or markets.
6. **Neutral research, separate strategy.** This library describes needs and evidence. What a specific product should do about them lives elsewhere. In practice:
    - Use only public sources, or sources that can be attributed openly. Anything learned in private conversations stays out.
    - Never assume a particular product. "What could serve this" sections compare kinds of product, and kinds of wallet (phone-based or always-online, payments or savings, iOS or Android), rather than judging one.
    - No scores or product-specific labels in research files.

## Say, do, make

Liz Sanders' framework for what to look at:

| | What it captures | Examples of sources |
| --- | --- | --- |
| **Say** | What people tell us | Interviews, surveys, comments, public calls for input |
| **Do** | What people actually do | Observation, transaction data, following a real process start to finish, public activity (listings, order threads) |
| **Make** | What people build to cope, or create when asked | Carrd pages, forms, spreadsheets, workarounds; money-flow maps and co-design sessions |

## Two levels of depth

**Quick scan** (one to two pages per area). Enough to judge the area and decide whether to go deeper:

1. **The question:** what this area asks, in one or two sentences.
2. **What's happening:** the strongest evidence of a real need, with sources. Include one line on **say versus do**: where what people say differs from what they actually do.
3. **Who:** the specific people or communities, as concretely as possible.
4. **Workarounds and players:** what people use today, and who else is building here.
5. **What could serve this:** the kinds of product that could meet the need, not only wallets: organizer and merchant tools, platforms, standards, services, games, physical objects. Then the trade-offs for each: where design matters, whether it works without custody or servers, platform (iOS, Android, web), amounts involved.
6. **Risks:** legal, Apple, reputation, technical.
7. **Confidence:** *low* (desk research only, few sources), *medium* (several solid sources) or *high* (direct research).
8. **Open questions:** what a deep dive would need to answer.
9. **Sources.**

**Deep dive** (a full document), following the community-driven economies file: thesis, definitions, why existing payments fail, case studies, sizing, what could serve this and the trade-offs for self-custodial, client-side products, risks and open questions, a say/do/make research plan, sources. Product-specific strategy is written separately.

## Evidence labels

Inline, in square brackets and italics:

- *[from memory]*: known but not checked in this research
- *[assumption]*: a guess or illustrative number, not data
- *[from earlier research]*: from a separate thread, not yet checked against originals
- *[to verify]*: worth checking before relying on it, including sources that couldn't be opened during the research

Anything without a label is linked to a source that was actually opened.

## File conventions

- `00`–`09`: entry points and foundation
- `11`–`29`: research areas, one file each (`NN-short-name.md`)
- `90`–`99`: cross-cutting research documents
- Each file starts with its title, a one-line status and a "last updated" date, and ends with sources.
