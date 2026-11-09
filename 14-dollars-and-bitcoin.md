# Dollars and bitcoin

*Quick scan. Confidence: medium on the market, low on merchants' reasons. Last updated November 9, 2026.*

## The question

Stablecoins are winning payments. Bitcoin builders hear it from merchants directly; merchants told one builder to "support USDT or go away" ([quoted by Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)). What do merchants and users actually mean when they ask for USDT? And how should bitcoin wallets handle people who want dollars: ignore it, display dollars, swap at the edges, or hold dollars on bitcoin rails?

## What's happening

**USDT on Tron is the default for stablecoin payments.**

- Artemis studied 31 stablecoin payment companies, a snapshot annualizing to $72.3 billion across business, peer-to-peer, consumer and card payments. USDT was 90% of payment volume, and Tron carried about 60% ([Yahoo Finance](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html), May 2025). Dragonfly's Rob Hadick said payment firms care little which chain settles, since Tron is fast and cheap, and that Tether is a trusted brand in places like Argentina and Brazil, where people worry about bank failures.
- Earlier scans found the same pattern for income: stablecoins were over 90% of crypto salaries in 2024 (area 12).

**Stablecoins can be, and are, frozen.** Tether froze more than $514 million in USDT across 370 addresses in the 30 days before May 8, 2026, about 98% of it on Tron. In 2025, 4,163 addresses were blacklisted with $1.26 billion frozen ([Cointelegraph on BlockSec data](https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show)). Most freezes target illicit activity, but the power is the issuer's.

**Dollars are arriving on bitcoin rails.**

- **Lightning:** Tether announced USDT on bitcoin and Lightning through Taproot Assets in January 2025 ([The Block](https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership)). It went live in March 2026, but the ecosystem is "still nascent," mostly LND-based, with early adoption through Speed Wallet and LnFi; the report gives no volumes ([Spark research](https://spark.money/research/lightning-network-2026-state)).
- **Ark:** Tether backed Ark Labs' $5.2 million seed round in March 2026 to expand stablecoin support on Arkade, the other main Ark implementation ([The Block](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin)). As of November 2026, Second hasn't announced plans for stablecoins in Bark. *[to verify]*
- **Bitcoin wallets with a dollar balance:** Blink offers a Dollar Balance, custodial through Stablesats or non-custodial with supported stablecoins ([Blink](https://www.blink.sv/en/dollar-balance)). The Breez SDK offers a "stable balance" that converts received sats to a stablecoin ([Breez SDK docs](https://sdk-doc-spark.breez.technology/guide/stable_balance.html)). Wallet of Satoshi added stablecoins to its self-custodial version, in beta from July 2026 and switched on in September, according to secondary reports ([Coin-Turk](https://en.coin-turk.com/wallet-of-satoshi-launches-stablecoins-on-lightning-with-self-custody-option/), [Stacker News](https://stacker.news/items/1561905)). *[to verify: official Wallet of Satoshi announcement]*

**Say versus do:** merchants *say* "support USDT." What they *do* is settle in USDT on Tron, mostly through payment companies, without caring much about the chain. That suggests they want *stable dollars their counterparties already use*, not USDT as such. Nobody has asked them directly what would make them accept something else.

## Who

| Group | What they want | Notes |
| --- | --- | --- |
| Merchants and sellers in emerging markets | Stable value, the currency their customers and suppliers already have | The "support USDT" voice; reasons not yet researched |
| People saving in weak-currency countries | Dollars that a bank can't fail on | Tether as a trusted brand (Argentina, Brazil) |
| Earners paid in stablecoins | Dollar income, sometimes with some bitcoin | Area 12 |
| Bitcoin holders paying people who want dollars | Pay in bitcoin, recipient gets dollars | Swaps at the edge |

## What could serve this

**Kinds of product**

- **Wallet stances** toward dollars (below).
- **Swap services** between bitcoin and stablecoins or local money (Boltz, SSPS providers; area 18).
- **Merchant tools** that accept one currency and settle in another.
- **Pricing tools:** displaying local currency and locking rates in invoices and orders.

**Trade-offs for wallets**

Four possible stances for a bitcoin wallet, from purest to most flexible:

1. **Bitcoin only:** amounts in sats or ₿, nothing else.
2. **Dollar display:** show prices in local currency, and lock the rate when an order or invoice is created. No dollar holdings.
3. **Swaps at the edges:** hold bitcoin, but pay someone who wants stablecoins, or get paid by someone who only has stablecoins (SSPS points this way, see area 18).
4. **A dollar balance:** hold dollars on bitcoin rails (Taproot Assets on Lightning, stablecoins on Ark), next to bitcoin.

The design problem is real at every step: two currencies in one wallet, without confusing people about what they hold.

## Risks

- **Issuer risk:** stablecoins bring back an issuer who can freeze funds, which undercuts self-custody.
- **Regulation:** stablecoin rules (GENIUS Act in the US, Brazil's settlement ban) change quickly.
- **Immaturity:** dollar rails on bitcoin are early, with few wallets and little liquidity.
- **Identity:** for wallets built around bitcoin, adding dollars can blur what they stand for.

## Open questions for a deep dive

1. When merchants ask for USDT, what do they need: stable value, their counterparties' currency, a dollar savings account, or simplicity? (Interviews and money-flow mapping.)
2. Would swaps at the edges satisfy them, or do they need to *hold* dollars?
3. How do people react to frozen stablecoins? Does it change behavior?
4. Which dollar rails on bitcoin will actually have liquidity in 2027: Taproot Assets, Arkade, Spark, or others? For a bitcoin-only wallet, which of them can it swap with at the edges?
5. What do bitcoin wallets that added dollars (Blink, Speed) see in usage: do people move into bitcoin over time, or stay in dollars?

## See also

[Stablecoins, unpacked](03-stablecoins.md) for the full picture, including non-dollar stablecoins and why most people outside dollarizing economies want stability in their own currency.

## Sources

- [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)
- [Yahoo Finance on the Artemis stablecoin payments report](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html)
- [Cointelegraph on Tether freezes (BlockSec data)](https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show)
- [The Block on USDT on Lightning](https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership)
- [Spark: State of the Lightning Network in 2026](https://spark.money/research/lightning-network-2026-state)
- [The Block on Tether backing Ark Labs](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin)
- [Blink Dollar Balance](https://www.blink.sv/en/dollar-balance)
- [Breez SDK: Stable Balance](https://sdk-doc-spark.breez.technology/guide/stable_balance.html)
- [Coin-Turk on Wallet of Satoshi stablecoins](https://en.coin-turk.com/wallet-of-satoshi-launches-stablecoins-on-lightning-with-self-custody-option/)
- [Stacker News on Wallet of Satoshi enabling stablecoins](https://stacker.news/items/1561905)
