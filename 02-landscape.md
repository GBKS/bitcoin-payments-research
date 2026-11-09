# Landscape

*The shared context for every area document, so they don't each repeat it. Last updated November 9, 2026.*

The question behind this library (why so few people pay with bitcoin, when the technology works) came from a year of conversations at bitcoin conferences. Spiral's two recent posts arrived while this thinking was underway. They reach a similar diagnosis, which is why they're summarized here as useful context, not as the starting point.

## Spiral: The Long Road to Bitcoin Payments

[The report](https://github.com/spiralxyz/bitcoin-payments), published in October 2026 as a GitHub repo and a post, is a call for moonshot ideas.

**The diagnosis.** Bitcoin payment technology has improved dramatically in seven years: Lightning runs in production, self-custodial wallets hide most of their complexity, and a first version of a payments app can be built from a single prompt to an AI coding tool. Yet few people pay with bitcoin in everyday life. "The gap is mostly demand, not technology."

**Why now.** Large payment companies are updating their rails, and they're choosing stablecoins: Shopify added USDC checkout, Stripe bought Bridge, and Open USD was announced in June 2026 with Stripe, Visa, American Express, Google and more than 140 others. About 99% of payments over Coinbase's x402 agent protocol are in USDC. If these early choices stick, bitcoin's absence now could be hard to reverse.

**The blockers**

- **Demand:** almost nobody is paid in bitcoin, so spending means buying first. Holders would rather save. Bitcoin's culture celebrates holding ("never sell your bitcoin"), and "bitcoin" carries baggage with mainstream users. Merchants see too few customers, and new platforms such as AI agents leave it out. Stablecoin issuers can share yield with partners; bitcoin can't.
- **Volatility and competition:** stablecoins meet the need for stable dollar payments directly, and offer programmability.
- **Policy:** in the US every purchase is a taxable sale, and the CLARITY Act stalled in September 2026.

**The comparison with stablecoins.** Bitcoin leads on what makes money open: no freezing, no blocking, no issuer, fixed supply. On ease of use it has "largely caught up." Stablecoins lead on what most people care about today: stable value, broad acceptance and policy, which are also where bitcoin has moved least.

**Four possible paths**

1. **Shared rails:** dollars or bitcoin over the same Lightning network. Lightning in agent payments, bitcoin on by default in fintech apps, and "lead with the payment, not the asset."
2. **Payments for people who need them most:** self-custodial payments for people facing capital controls or unstable currencies.
3. **New reasons to spend:** incentives for existing holders.
4. **New ways to spend:** new kinds of payments, such as paying creators or AI services per use, streaming payments, and "bolder experiments" that generate demand. "The killer app for micropayments probably won't feel like a traditional payment at all."

**How Spiral would measure success:** how many customers spend bitcoin, how often they pay again, the number, value and share of payments funded in bitcoin, and whether use continues after incentives end. Bitcoin used only to route dollar payments doesn't count.

## Spiral: Value Stored. Now What?

[Spiral's summary of findings](https://spiralxyz.substack.com/p/value-stored-now-what) (Conor Okus, November 4, 2026) draws on hundreds of ideas from GitHub, X, Stacker News and elsewhere, with the strongest collected in the [GitHub discussion](https://github.com/spiralxyz/bitcoin-payments/discussions/1).

**The headline:** help people and businesses **earn** and hold bitcoin, not just spend it. Market bitcoin as "something you get paid in rather than something you immediately spend."

**What the community agreed on:** demand, not technology, is the main gap. Volatility and familiarity with dollar prices remain barriers. Earning before spending was the most repeated point. Stablecoins are winning: merchants told MegalithicBTC to "support USDT or go away," and issuers can share reserve yield with partners and customers. On X, the most common reply called for tax exemptions on small payments.

**Three areas that could move bitcoin payments in the next five years**

1. **Global entrepreneurs, human or agent, earning in bitcoin.** The strongest support. Cross-border sellers rely on bank wires because cards bring fees, chargebacks, slow settlement and reserves. Lightning offers instant, final, low-fee settlement. Wallets and providers could offer bitcoin income through wage conversion, gig payouts and automatic rewards. Examples: [Trails Coffee](https://trailscoffee.com/) and [BitTasker](https://bittasker.com/).
2. **Agentic payments.** Agents already buy services over L402. Builders could run experiments where agents *earn* bitcoin for useful work, measured against x402 and stablecoin flows.
3. **Self-custody as stablecoins get more regulated and freezable.** Bitcoin can't be frozen or seized, so demand may grow among businesses in weak-currency countries or with frozen stablecoins. Possible catalysts: a US crackdown on providers that don't KYC stablecoin wallets, and countries restricting dollar stablecoins, as [Brazil's central bank did for cross-border settlement](https://www.coindesk.com/policy/2026/05/02/brazil-s-central-bank-bans-stablecoin-and-crypto-settlement-in-cross-border-payments). Bitcoin-based stablecoin rails such as Ark and Taproot Assets are immature and need investment.

## Where this library differs from Spiral's framing

- **Products, not just protocols.** Most of the ecosystem's attention goes to infrastructure. This library treats products and design as a primary lever for demand.
- **Do and make, not only say.** The call for input mostly captured opinions, largely from builders. Several open questions (such as why merchants want USDT) need direct research.
- **Beyond merchants and remittances.** Community economies, gray markets and subcultures are underexplored, partly because they're less respectable to talk about.

## Bitcoin payments in numbers

- **Merchant acceptance is mostly a map, not a market.** BTC Map listed 26,914 bitcoin-accepting merchants on August 31, 2026, but only 16,243 (about 60%) had been verified within the past year ([BTC Map](https://blog.btcmap.org/posts/2026-08/)).
- **Acceptance stopped being the bottleneck in the US.** On March 30, 2026, Square turned on Lightning payments by default for about four million US merchants (outside New York), with zero fees through 2026 and 1% after. Merchants can settle in dollars, keep everything in bitcoin, or keep a percentage ([Whale Alert](https://whale-alert.io/stories/bb9e015c075f35/Block-auto-enables-native-Bitcoin-Lightning-payments-for-4M-Square-merchants-zero-processing-fees-through-2026-merchants-may-settle-in-USD-BTC-or-a-percentage)).
- **Bitcoin is how people enter crypto, not how they pay.** Chainalysis's 2025 index found bitcoin drew over $4.6 trillion in fiat inflows, against just under $1 trillion for stablecoins. The top countries were India, the US, Pakistan, Vietnam and Brazil ([Cointelegraph](https://cointelegraph.com/news/us-second-in-crypto-adoption-india-leads-all-chainalysis), September 2025).
- **Lightning:** USDT on Lightning went live in March 2026 but remains nascent, mostly LND-based ([Spark research](https://spark.money/research/lightning-network-2026-state)).

## The cost baseline

Sending $200 abroad costs 6.36% on average worldwide and 8.46% to sub-Saharan Africa, the most expensive region. Banks charge 14.99% on average; digital services 4.59%; the three cheapest services per corridor average 3.29% ([African Exponent on World Bank data](https://www.africanexponent.com/chart-of-the-day-sending-200-home-to-sub-saharan-africa-costs-8-46-percent/), Q3 2025). This is what any claim that bitcoin is cheaper across borders competes with.

## Stablecoins in brief

About $288 billion in total, 99% in dollars, 85% in just USDT and USDC. Actual payments are roughly 1% of headline volume, and increasingly domestic. Outside dollarizing economies, most people want stability in their *own* currency, not dollars. Full picture, including a tracker of announced versus live projects: [Stablecoins, unpacked](03-stablecoins.md).

## Lessons from payment systems that took off

*A growing section. Bitcoin's demand problem has been solved, for other money, several times.*

### Pix in Brazil

Paulo Sacramento, a UX researcher in the Bitcoin Design Community, studied 25 people in Rio de Janeiro and Viçosa in August and September 2022: interviews in homes and workplaces, paying vendors with Pix, receiving payments, photos and field notes ([Pix in Brazil: a field study for the Bitcoin community](https://www.psacramento.com/pix-in-brazil-a-field-study-for-the-bitcoin-community/), March 2024).

**Why it spread:** instant settlement, zero fees for individuals (some said they'd stop if fees came in), simple aliases or QR codes, and broad acceptance. But features alone don't explain it: high smartphone use, a large informal economy, dense messaging networks and a government-led legal framework and public education all played a part. Merchants describe Pix as a business necessity; it avoids card terminals and the problem of making change.

**What went wrong:**

- **Personal identifiers as payment keys.** Using a phone number, email or national ID number as a payment address breaks compartmentalization; leaked keys and data led to scams, and payment confirmations show the payer's name, partial ID number and bank.
- **Paying the wrong person** with similar contact names, especially in a hurry.
- **Fake receipts:** scheduled payments or edited screenshots shown as completed, judged by sellers at a glance.
- **No credit:** instant settlement can't replace installment payments that many Brazilians rely on.
- **Older adults** made up about 4% of transactions and often rely on a family member to help.

**Lessons the study draws for bitcoin:** build bridges to national payment systems rather than treating them as threats; market to merchants on no hardware, low fees and no change; present bitcoin as "the money you do not need to carry around"; avoid phone numbers and emails as payment identifiers; design for clear contacts (identicons, history, warnings for similar names); make receipts verifiable at a glance (a live timer, an emoji derived from the payment proof); design for the family members who help older users.

**Relevance across the library:** phone numbers as payment addresses (area 18, Tando) carry Pix's privacy risks. Verifiable receipts matter for group orders and fan projects (area 11). Bridges to national systems are the last-mile pattern (area 18).

### Still to research

- **UPI in India:** government-built, zero fees, the largest real-time payment system by volume. *[to research]*
- **M-Pesa in Kenya:** agent networks and trust in a mobile operator. *[to research]*
- **WeChat Pay and Alipay:** rituals, super-apps and QR codes (red envelopes in area 16). *[to research]*

## How the areas map

| Area | Spiral report | Spiral summary |
| --- | --- | --- |
| 11 [Community-driven economies](11-community-driven-economies.md) | New ways to spend | Earning (organizers, creators) |
| 12 [Earning in bitcoin](12-earning-in-bitcoin.md) | (Blocker: nobody is paid in bitcoin) | Area 1 |
| 13 [Agentic payments](13-agentic-payments.md) | Shared rails; new ways to spend | Area 2 |
| 14 [Dollars and bitcoin](14-dollars-and-bitcoin.md) | Shared rails; competition from stablecoins | Stablecoins winning; Lightning carrying dollars |
| 15 [Money that can't be frozen](15-money-that-cant-be-frozen.md) | Payments for people who need them most | Area 3 |
| 16 [Payments that feel different](16-payments-that-feel-different.md) | New ways to spend; streaming | — |
| 17 [Brand and culture as demand](17-brand-and-culture-as-demand.md) | Blocker: culture and marketing; lead with the payment | Market bitcoin as something you get paid in |
| 18 [Last-mile infrastructure](18-last-mile-infrastructure.md) | Shared rails | Rails for stablecoins (Ark, Taproot Assets) |

## Key projects and players

| Name | What | Relevance |
| --- | --- | --- |
| Second / Bark | Ark implementation | One of the two main Ark implementations, with Arkade (Ark Labs) *[from memory; to verify]* |
| [Spark](https://www.spark.money/) | Bitcoin payment layer for stablecoins and bitcoin | Named by Spiral as a newer self-custodial integration option |
| x402 (Coinbase), AP2 (Google), Machine Payments Protocol (Stripe) | Agent payment protocols, mostly stablecoin-based | The competition in agentic payments ([Spiral report](https://github.com/spiralxyz/bitcoin-payments)) |
| L402 | Lightning-based payments for APIs and agents *[from memory: Lightning Labs]* | Bitcoin's existing agent payment standard |
| [Kaleidoswap SSPS](https://github.com/kaleidoswap/ssps) | Draft protocol for choosing non-custodial swap providers across layers | Last-mile infrastructure |
| [Pave](https://gbks.substack.com/p/pave-protocol-for-last-mile-bitcoin) | A sketch by this library's author for paying phone numbers and bank accounts from a bitcoin wallet | Last-mile infrastructure |
| [Trails Coffee](https://trailscoffee.com/), [BitTasker](https://bittasker.com/) | Live projects where people earn bitcoin | Earning; possible research partners |
| [KDOL](https://en.wowtale.net/2025/10/09/232389) (Hashpurple) | Crowdfunding for K-pop fan ads, not crypto-based | Reference product for community economies |
| Cash App / Square | Lightning on by default for about four million US Square merchants since March 2026 | Design and brand comparison; Spiral is part of Block |
| CoinOS, a Japanese bitcoin community | Run their own Ark servers *[from memory; to verify]* | Server diversity for Ark |
| Taproot Assets | Stablecoins on bitcoin *[from memory: Lightning Labs]* | Dollars and bitcoin |

## Sources

- [Pix in Brazil: a field study for the Bitcoin community](https://www.psacramento.com/pix-in-brazil-a-field-study-for-the-bitcoin-community/)
- [BTC Map: global metrics, August 2026](https://blog.btcmap.org/posts/2026-08/)
- [Whale Alert on Square's Lightning rollout](https://whale-alert.io/stories/bb9e015c075f35/Block-auto-enables-native-Bitcoin-Lightning-payments-for-4M-Square-merchants-zero-processing-fees-through-2026-merchants-may-settle-in-USD-BTC-or-a-percentage)
- [Cointelegraph on Chainalysis's 2025 index](https://cointelegraph.com/news/us-second-in-crypto-adoption-india-leads-all-chainalysis)
- [African Exponent on World Bank remittance prices](https://www.africanexponent.com/chart-of-the-day-sending-200-home-to-sub-saharan-africa-costs-8-46-percent/)

- [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments)
- [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)
- [Spiral GitHub discussion](https://github.com/spiralxyz/bitcoin-payments/discussions/1)
- [CoinDesk on Brazil's stablecoin settlement ban](https://www.coindesk.com/policy/2026/05/02/brazil-s-central-bank-bans-stablecoin-and-crypto-settlement-in-cross-border-payments)
