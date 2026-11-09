# Pilot audit: Dollars and bitcoin

*Auto-research pilot, step 4. Prepared and audited November 9, 2026. Verdicts as checked before the page edits; see `14-dollars-and-bitcoin.yml` for the current records.*

**Your call** records the author's audit of each verdict. Details for every claim, with the sources and quotes each checker used, are below the table.

**Legend.** A is the checker that saw the claims file; B is the independent rechecker that saw only claim text and source. *Quote* shows whether each quote was found verbatim on the source page by a script: ✓ found, – no quote given, 403 the site blocks scripts, so it couldn't be checked.

| Claim | Page text | A | B | Quote A / B | Proposed | Your call |
| --- | --- | --- | --- | --- | --- | --- |
| 14-01 | one told a builder to "support USDT or go away" | partly | verified | ✓ / ✓ | Change "one told a builder" to "merchants told a builder". The same wording is in Landscape ("one merchant told MegalithicBTC"). | agree |
| 14-02 | Artemis studied 31 stablecoin payment companies | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-03 | a snapshot annualizing to $72.3 billion | verified | verified | ✓ / ✓ | Optional: the source also lists lending among the payment types. | agree |
| 14-04 | USDT was 90% of payment volume | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-05 | Tron carried about 60% | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-06 | May 2025 | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-07 | Dragonfly's Rob Hadick said payment firms care little which chain settles, since Tron is fast and cheap | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-08 | Tether is a trusted brand in places like Argentina and Brazil, where people worry about bank failures | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-09 | stablecoins were over 90% of crypto salaries in 2024 | unreachable | verified | – / ✓ | Keep. Only checker B could read it (archived copy). | agree |
| 14-10 | Tether froze more than $514 million in USDT | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-11 | across 370 addresses | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-12 | in the 30 days before May 8, 2026 | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-13 | about 98% of it on Tron | verified | verified | ✓ / ✓ | Keep. 98% is calculated by value ($505.9M of $514.6M); by address count it's about 89%. | agree |
| 14-14 | In 2025, 4,163 addresses were blacklisted | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-15 | with $1.26 billion frozen | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-16 | Tether announced USDT on bitcoin and Lightning through Taproot Assets in January 2025 | verified | verified | 403 / 403 | Keep. | agree |
| 14-17 | It went live in March 2026 | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-18 | the ecosystem is "still nascent," | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-19 | mostly LND-based | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-20 | early adoption through Speed Wallet and LnFi | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-21 | no published volumes | partly | unsourced | – / – | Change "no published volumes" to "the report gives no volumes". | agree |
| 14-22 | Tether backed Ark Labs' $5.2 million seed round | verified | verified | 403 / 403 | Keep. | agree |
| 14-23 | seed round in March 2026 | verified | verified | 403 / 403 | Keep. March 2026 is when the raise was announced. | agree |
| 14-24 | to expand stablecoin support on Arkade | verified | verified | 403 / 403 | Keep. | agree |
| 14-25 | Second hasn't announced plans for stablecoins in Bark. | unsourced | unsourced | – / – | Keep *[to verify]*; add "as of November 2026". | agree |
| 14-26 | Blink offers a Dollar Balance | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-27 | custodial through Stablesats or non-custodial with supported stablecoins | verified | verified | ✓ / ✓ | Keep. | agree |
| 14-28 | Breez SDK's "stable balance" | verified | verified | ✓ / ✓ | Link the Breez SDK Stable Balance docs and drop this part of the label. | agree |
| 14-29 | Wallet of Satoshi's stablecoin plans | partly | partly | ✓ / ✓ | Update: reportedly launched in September 2026 in the self-custodial version; secondary sources only, so keep a *[to verify: official announcement]* label. | agree |

## Measures

| Measure | Result |
| --- | --- |
| Extraction completeness | 25 of the 27 clear claims on a baseline list written before seeing the agent's list (93%). Missed: "most freezes target illicit activity" and "Arkade, the other main Ark implementation"; the agent left both out deliberately and said so. |
| Agreement between checkers | 26 of 29 verdicts identical. The 3 differences are labeling (14-01, 14-21) or access (14-09), not substance. |
| Made-up quotes | None. Every quote that could be fetched was found verbatim: 22 of 26 (A) and 23 of 27 (B); the other 4 each come from The Block, which returns 403 to scripts, so claims 14-16 and 14-22 to 14-24 can't be checked mechanically. |
| Unreachable sources | The Block (2 articles) blocks scripts; Blockworks blocks both agents and scripts (B used an archived copy). |
| Verdict accuracy | 29 of 29 (100%): the author agreed with every verdict. |
| Author's time | About 15 minutes for the audit. Time to check by hand: not yet estimated. |

## Claim details

### 14-01

**Page:** one told a builder to "support USDT or go away"

- **A (partly):** Quote is correct, but Spiral says merchants (plural) told the builder (the account MegalithicBTC), not one merchant. Suggest: 'merchants told a builder to "support USDT or go away"'.
  - Source: https://spiralxyz.substack.com/p/value-stored-now-what
  - Quote: “to “support USDT or go away.” Stablecoins also have an economic edge”
- **B (verified):** Spiral attributes the line to merchants (plural) speaking to the builder MegalithicBTC; the claim's 'one' is a slight simplification.
  - Source: https://spiralxyz.substack.com/p/value-stored-now-what
  - Quote: “merchants told MegalithicBTC to “support USDT or go away.””

### 14-02

**Page:** Artemis studied 31 stablecoin payment companies

- **A (verified):** Artemis report (with Dragonfly and Castle Island) covered 31 stablecoin payment companies.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “looked at data from 31 stablecoin payment companies, and found USDT, the largest stablecoin, accounted for 90 percent of payment transaction volume”
- **B (verified):** Artemis report 'Stablecoin Payments from the Ground Up', with Dragonfly and Castle Island Ventures.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “looked at data from 31 stablecoin payment companies”

### 14-03

**Page:** a snapshot annualizing to $72.3 billion

- **A (verified):** Matches. Minor: the source's categories also include Lending (B2B, P2P, B2C, Card, Lending), which the page's list omits; snapshot was taken in February 2025.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “The snapshot of stablecoin payment volume taken in February added up to an annualized $72.3 billion”
- **B (verified):** The snapshot was taken in February 2025 and annualized.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “added up to an annualized $72.3 billion”

### 14-04

**Page:** USDT was 90% of payment volume

- **A (verified):** Source says USDT was 90 percent of payment transaction volume.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “accounted for 90 percent of payment transaction volume, followed by Circle's USDC, the second-largest”
- **B (verified):** USDT share of payment volume among the 31 companies.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “accounted for 90 percent of payment transaction volume”

### 14-05

**Page:** Tron carried about 60%

- **A (verified):** Matches.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “Tron was the preferred settlement network, hosting around 60 percent of volume”
- **B (verified):** Tron as the preferred settlement network.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “hosting around 60 percent of volume”

### 14-06

**Page:** May 2025

- **A (verified):** Article dated May 29, 2025 (Ian Allison). The underlying data snapshot is from February 2025.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “May 29, 2025”
- **B (verified):** Article (and report coverage) dated May 29, 2025; note the underlying data snapshot was taken in February 2025.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “May 29, 2025”

### 14-07

**Page:** Dragonfly's Rob Hadick said payment firms care little which chain settles, since Tron is fast and cheap

- **A (verified):** Reported speech attributed to Hadick ('he added'); Hadick is Dragonfly general partner.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “Moreover, firms that use stablecoins for payments have little concern about which blockchain is being used to settle on. Tron is fast and cheap”
- **B (verified):** Attributed to Dragonfly general partner Rob Hadick; the article also cites over $60 billion of USDT on Tron as a reason.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “firms that use stablecoins for payments have little concern about which blockchain is being used to settle on. Tron is fast and cheap”

### 14-08

**Page:** Tether is a trusted brand in places like Argentina and Brazil, where people worry about bank failures

- **A (verified):** Matches; attributed to Hadick.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “places like Argentina or Brazil, for instance, people might be worried about things like bank failures, and Tether is seen as a trusted brand”
- **B (verified):** Hadick's view; the source hedges ('might be worried'), which the claim's 'worry' slightly firms up.
  - Source: https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html
  - Quote: “people might be worried about things like bank failures, and Tether is seen as a trusted brand”

### 14-09

**Page:** stablecoins were over 90% of crypto salaries in 2024

- **A (unreachable):** The source linked from area 12 (Blockworks on Pantera's survey) returned HTTP 403 to both curl and WebFetch; not checked. An archive copy was not used.
  - Source: https://blockworks.co/news/stablecoins-salaries-2024-pantera-survey
  - Quote: (none)
- **B (verified):** Live Blockworks page returned 403; checked via the Wayback Machine copy (Blockworks, Aug 6, 2025, citing Pantera's compensation survey). The 90%+ is USDC plus USDT; headline says 90%.
  - Source: https://web.archive.org/web/2025/https://blockworks.co/news/stablecoins-salaries-2024-pantera-survey
  - Quote: “USDC (63%) and USDT (28.6%) collectively account for over 90% of crypto salaries”

### 14-10

**Page:** Tether froze more than $514 million in USDT

- **A (verified):** Matches (BlockSec USDT Freeze Tracker data).
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether has frozen more than $514 million in USDT across Ethereum and Tron over the past 30 days”
- **B (verified):** BlockSec USDT Freeze Tracker data, as reported by Cointelegraph.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether has frozen more than $514 million in USDT across Ethereum and Tron over the past 30 days”

### 14-11

**Page:** across 370 addresses

- **A (verified):** Matches.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “the tool shows 370 addresses blacklisted in that period, including 328 on Tron and 42 on Ethereum”
- **B (verified):** 328 on Tron and 42 on Ethereum.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “370 addresses blacklisted in that period”

### 14-12

**Page:** in the 30 days before May 8, 2026

- **A (verified):** Article published May 8, 2026 (a Friday) and describes 'the past 30 days' as of Friday, so the window is the 30 days to May 8, 2026.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “May 8, 2026”
- **B (verified):** Article published May 8, 2026 (page metadata and dateline), with figures 'as of Friday'.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether has frozen more than $514 million in USDT across Ethereum and Tron over the past 30 days”

### 14-13

**Page:** about 98% of it on Tron

- **A (verified):** Derived, not stated: $505.9M of about $514.6M is about 98.3% on Tron. The page's 'about 98%' is correct arithmetic. (By address count, Tron is 328 of 370, about 89%.)
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “with about $505.9 million frozen on Tron and $8.73 million on Ethereum”
- **B (verified):** 98% is a calculation: 505.9 / (505.9 + 8.73) = about 98.3%; the article does not state the percentage itself.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “about $505.9 million frozen on Tron and $8.73 million on Ethereum”

### 14-14

**Page:** In 2025, 4,163 addresses were blacklisted

- **A (verified):** Matches (BlockSec analysis of 2025 data).
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether blacklisted 4,163 unique addresses across Ethereum and Tron, freezing a total of $1.26 billion in USDT”
- **B (verified):** From BlockSec's analysis of 2025 data.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether blacklisted 4,163 unique addresses across Ethereum and Tron, freezing a total of $1.26 billion in USDT”

### 14-15

**Page:** with $1.26 billion frozen

- **A (verified):** Matches.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether blacklisted 4,163 unique addresses across Ethereum and Tron, freezing a total of $1.26 billion in USDT”
- **B (verified):** Figure is for 2025.
  - Source: https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show
  - Quote: “Tether blacklisted 4,163 unique addresses across Ethereum and Tron, freezing a total of $1.26 billion in USDT”

### 14-16

**Page:** Tether announced USDT on bitcoin and Lightning through Taproot Assets in January 2025

- **A (verified):** Dated January 30, 2025; article says the integration is supported by Taproot Assets. The Block returns 403 to curl; text was read via WebFetch only, so an automated quote check may fail.
  - Source: https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership
  - Quote: “Stablecoin issuer Tether plans to bring its token USDT onto the Bitcoin base layer and Layer 2 protocol Lightning Network.”
- **B (verified):** Curl got 403, WebFetch worked. Article dated January 30, 2025; it says the integration is supported by Taproot Assets (Lightning Labs).
  - Source: https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership
  - Quote: “Stablecoin issuer Tether plans to bring its token USDT onto the Bitcoin base layer and Layer 2 protocol Lightning Network”

### 14-17

**Page:** It went live in March 2026

- **A (verified):** Matches.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Tether announced USDT support on Bitcoin and Lightning in January 2025, with the integration going live in March 2026”
- **B (verified):** Single secondary source (Spark, itself a competing Layer 2); no primary Tether launch announcement was checked.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Tether announced USDT support on Bitcoin and Lightning in January 2025, with the integration going live in March 2026”

### 14-18

**Page:** the ecosystem is "still nascent,"

- **A (verified):** Exact wording 'still nascent' is in the source.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Early adoption is happening through wallets like Speed Wallet and LnFi, though the ecosystem is still nascent”
- **B (verified):** Exact wording 'still nascent' appears.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Early adoption is happening through wallets like Speed Wallet and LnFi, though the ecosystem is still nascent”

### 14-19

**Page:** mostly LND-based

- **A (verified):** Source says 'primarily LND-based'; page says 'mostly'. Same meaning.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Stablecoin support on Lightning is new and limited to implementations using Taproot Assets (primarily LND-based infrastructure)”
- **B (verified):** Source says 'primarily LND-based', matching 'mostly'.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “limited to implementations using Taproot Assets (primarily LND-based infrastructure)”

### 14-20

**Page:** early adoption through Speed Wallet and LnFi

- **A (verified):** Matches.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Early adoption is happening through wallets like Speed Wallet and LnFi, though the ecosystem is still nascent”
- **B (verified):** 
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: “Early adoption is happening through wallets like Speed Wallet and LnFi, though the ecosystem is still nascent”

### 14-21

**Page:** no published volumes

- **A (partly):** The Spark report gives no volume figures for stablecoins on Lightning, but it doesn't say that none are published. A web search (Nov 9, 2026) found only an unsourced opinion-piece figure, no official data. Suggest: 'and the Spark report gives no volumes'.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: (none)
- **B (unsourced):** The Spark article gives no volume figures for stablecoins on Lightning, but it does not say that none are published; the claim is an inference from absence.
  - Source: https://spark.money/research/lightning-network-2026-state
  - Quote: (none)

### 14-22

**Page:** Tether backed Ark Labs' $5.2 million seed round

- **A (verified):** Tether was one of several backers (also Ego Death Capital, Epoch VC and others). Read via WebFetch only; The Block returns 403 to curl.
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “Ark Labs has raised $5.2 million in a seed funding round”
- **B (verified):** Curl got 403, WebFetch worked. The article says the round included backing from Tether, among other investors.
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “Ark Labs has raised $5.2 million in a seed funding round to expand infrastructure”

### 14-23

**Page:** seed round in March 2026

- **A (verified):** Article dated March 12, 2026 (date read via WebFetch; quote is for the round, not the date).
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “Ark Labs has raised $5.2 million in a seed funding round”
- **B (verified):** Announced March 12, 2026. Caveat: the article says Ark Labs did not disclose when the round was raised, so 'March 2026' is the announcement date.
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “March 12, 2026, 9:00AM EDT”

### 14-24

**Page:** to expand stablecoin support on Arkade

- **A (verified):** Close: the source ties the round to the launch of stablecoin support on Arkade, and the headline says it will 'expand stablecoin and programmable finance infrastructure'.
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “The funding announcement also coincides with the launch of stablecoin and other digital asset support on Arkade”
- **B (verified):** Headline frames the raise as expanding stablecoin and programmable finance infrastructure on bitcoin.
  - Source: https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin
  - Quote: “The funding coincides with Arkade adding support for stablecoins”

### 14-25

**Page:** Second hasn't announced plans for stablecoins in Bark.

- **A (unsourced):** Absence claim. As of Nov 9, 2026: no mention of stablecoins, USDT or Taproot Assets on the second.tech, blog.second.tech and docs.second.tech front pages, and web searches found none. Coverage of Bark's mainnet launch (June 2026) describes bitcoin payments only. Can't prove a negative; the [to verify] label is appropriate.
  - Source: https://second.tech/
  - Quote: (none)
- **B (unsourced):** As of Nov 9, 2026 no stablecoin announcement for Bark was found: checked Second's blog index, second.tech, docs.second.tech and the Bark mainnet launch post (June 2026), plus web searches. Absence only, not a source stating it.
  - Source: https://blog.second.tech/bark-now-on-bitcoin-mainnet/
  - Quote: (none)

### 14-26

**Page:** Blink offers a Dollar Balance

- **A (verified):** Matches.
  - Source: https://blink.sv/en/dollar-balance
  - Quote: “Dollar Balance is Blink’s USD-denominated balance feature.”
- **B (verified):** Blink's own page describes Dollar Balance as its USD-denominated balance feature.
  - Source: https://blink.sv/en/dollar-balance
  - Quote: “It is designed for people who want to use Blink for everyday payments without taking on bitcoin price volatility”

### 14-27

**Page:** custodial through Stablesats or non-custodial with supported stablecoins

- **A (verified):** Matches. The page links Spark.money for the non-custodial mode, so the stablecoins appear to run on Spark [inferred from the link, not stated].
  - Source: https://blink.sv/en/dollar-balance
  - Quote: “In Custodial Mode, Dollar Balance is powered by Stablesats. In Non-Custodial Mode, Dollar Balance uses supported stablecoins on the non-custodial protocol.”
- **B (verified):** The page links Spark.money for the non-custodial mode.
  - Source: https://blink.sv/en/dollar-balance
  - Quote: “In Custodial Mode, Dollar Balance is powered by Stablesats. In Non-Custodial Mode, Dollar Balance uses supported stablecoins on the non-custodial protocol.”

### 14-28

**Page:** Breez SDK's "stable balance"

- **A (verified):** Proposed source: the Breez SDK (Spark) docs describe 'Stable Balance', which converts received sats to a stablecoin such as USDB. The page's [to verify] label could be replaced with this link.
  - Source: https://sdk-doc-spark.breez.technology/guide/stable_balance.html
  - Quote: “The stable balance feature enables users to switch between bitcoin and a stablecoin, like”
- **B (verified):** Breez SDK docs have a 'Stable Balance' feature (example token USDB). Bitcoin Magazine (Sept 2026) also refers to Breez's 'stable balance feature'.
  - Source: https://sdk-doc-spark.breez.technology/guide/stable_balance.html
  - Quote: “On receive, sats are automatically converted to the stablecoin. On send, the stablecoin is converted to Bitcoin.”

### 14-29

**Page:** Wallet of Satoshi's stablecoin plans

- **A (partly):** The feature appears to have launched, so it is no longer only a plan: digital dollars in the self-custodial version, with USDC/USDT deposits from five networks. The only source found is a secondary Stacker News post, with no official Wallet of Satoshi announcement found. Suggest rewording to 'Wallet of Satoshi added stablecoins in September 2026' once an official source is found.
  - Source: https://stacker.news/items/1561905
  - Quote: “Wallet of Satoshi has enabled the stablecoin feature in its app, which it began testing in July, the development team announced on September 2, 2026.”
- **B (partly):** Wallet of Satoshi has gone beyond 'plans': it launched a stablecoin beta (self-custodial version) and a Stacker News post from early Sept 2026 reports it enabled after months in beta. Secondary sources only; no official WoS post checked.
  - Source: https://en.coin-turk.com/wallet-of-satoshi-launches-stablecoins-on-lightning-with-self-custody-option/
  - Quote: “Stablecoins on Lightning are now available in beta, allowing users to access dollars and Bitcoin together with self-custody in one app.”
