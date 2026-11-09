# Stablecoins, unpacked

*Foundation document. "Stablecoins" is used as if it were one competitor. It isn't. Last updated November 9, 2026.*

## Why this page

The word covers very different kinds of money: tokens from companies that can freeze them, bank deposits on a blockchain, synthetic dollars built from trading positions, tokenized gold, euros and yen. It mixes payments with trading. It counts announcements as adoption. And it assumes everyone wants dollars. This page separates those things, so claims like "stablecoins are winning" can be made precisely.

## Kinds of stablecoin

| Kind | Backed by | Who can freeze | Yield to holders | Examples | Size (Nov 8, 2026) |
| --- | --- | --- | --- | --- | --- |
| Company-issued, fiat-backed | Cash and short-term government debt held by the issuer | The issuer, often at government request | Not from issuers under US law; sometimes via third parties | USDT, USDC, PayPal USD, Ripple USD, Global Dollar, USD1 | Fiat-backed total about $274 billion |
| Consortium-issued | The same, with revenue shared among partner businesses | The managing organization | Shared with businesses, not holders | Open USD | About $0.9 billion |
| Bank-issued | Bank deposits | The bank | Possibly, as deposits | Various pilots | About $0.24 billion |
| Crypto-backed | Other crypto held as collateral in smart contracts | Varies; some have freeze functions | Sometimes, through savings modules | USDS, Dai, GHO | Crypto-backed total about $4.7 billion |
| Synthetic | Trading positions that offset price swings | Varies | Yes, from trading income | Ethena USDe | About $4.9 billion |
| Non-dollar fiat | Euros, yen, Swiss francs, real, pesos | The issuer | Generally no | EURC, JPYC, BRL tokens | Under $1.5 billion in total |
| Tokenized gold | Physical gold in vaults | The issuer | No | Tether Gold, PAX Gold | About $5.1 billion |
| Bitcoin-based synthetic dollars | Bitcoin plus a hedge, held by a service | The service, if custodial | No | Stablesats (Blink) | Small |

*Category sizes are CoinGecko's ([CoinGecko](https://www.coingecko.com/en/categories/stablecoins)), retrieved November 8, 2026. Categories overlap.*

## Size and concentration

- **Total:** about **$288 billion**, against bitcoin's market capitalization of about $1.53 trillion.
- **Dollars are almost everything:** dollar stablecoins are about $285 billion, **99%** of the total.
- **Two issuers dominate:** USDT about $177 billion (61%) and USDC about $70 billion (24%). The next largest, USDS, is under $9 billion.
- **Non-dollar stablecoins are tiny:** euro about $830 million, yen about $236 million, Swiss franc about $89 million, pound about $27 million, Korean won and Mexican peso under $1 million each.

*All CoinGecko, November 8, 2026.*

## Payments versus everything else

Headline figures overstate payments:

| Measure | Figure | Source |
| --- | --- | --- |
| All stablecoin transaction volume, past year | ~$46 trillion | a16z State of Crypto 2025 ([Finextra](https://www.finextra.com/blogposting/29723/deep-dive-what-a16zs-state-of-crypto-2025-really-says-about-stablecoins-and-ai)) |
| Adjusted for bots and wallet shuffling | ~$9 trillion | Same |
| Estimated actual payments, last year | $350–550 billion | Cited by [DigitalToday](https://www.digitaltoday.co.kr/en/view/51250/stablecoins-share-of-local-payments-rises-as-cross-border-use-fades), April 2026 |
| Payment companies studied by Artemis (31 firms, annualized) | ~$72 billion | [Yahoo Finance on Artemis](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html), 2025 |

So actual payments are roughly **1% of headline volume**. "Stablecoins process more than Visa" compares trading and treasury movements with card purchases.

**Payments are becoming local, not cross-border:** the domestic share of stablecoin transactions rose from about 50% in early 2024 to about 75% in early 2026, according to a16z's Robert Hackett and Jeremy Zhang ([DigitalToday](https://www.digitaltoday.co.kr/en/view/51250/stablecoins-share-of-local-payments-rises-as-cross-border-use-fades)).

## Where they run

- **Tron's share is falling** on some measures: from 36% of stablecoin transaction volume at the start of 2025 to 14.6% in February 2026, with Solana and Ethereum gaining, per Visa's onchain analytics ([ForkLog](https://forklog.com/en/trons-share-in-stablecoin-transactions-plummets-to-14/)).
- **But Tron still dominated payment companies' volume** (about 60%) in Artemis's 2025 study. Different measures, different answers: Tron remains the default for emerging-market payments, while other chains grow in overall volume.
- **New chains built for payments:** Stripe and Paradigm's Tempo launched on mainnet on March 18, 2026, with partners including Visa, Mastercard, Deutsche Bank, Shopify, OpenAI and Anthropic. No usage figures have been published ([DEV Community](https://dev.to/tomwangcn/stripe-tempo-goes-live-ai-agent-payment-rails-3306)).

## Announced, live, used

| Project | What | Status | Signs of use |
| --- | --- | --- | --- |
| **Open USD** | Consortium stablecoin by Open Standard, 140+ backers including Visa, Stripe, Mastercard, BlackRock, Coinbase; reserve income shared with participating businesses; fee-free minting and redemption; natively on Tempo ([The Block](https://theblock.co/post/406736/visa-stripe-coinbase-join-open-usd-stablecoin-shares-reserve-revenue)) | Announced June 2026; listed on CoinGecko by November *[to verify: launch date]* | About $0.9 billion market cap |
| **Tempo** | Payments chain by Stripe and Paradigm | Live since March 18, 2026 | No published figures |
| **PayPal USD** | PayPal's stablecoin | Live | About $2.8 billion |
| **Ripple USD, Global Dollar, USD1** | Company-issued dollar tokens | Live | About $2.7, $2.7 and $3.4 billion |
| **JPYC** | First regulated yen stablecoin, under Japan's revised Payment Services Act, launched October 27, 2025; target ¥10 trillion in three years ([Unlock](https://unlock-bc.com/en/japan-launches-worlds-first-regulated-yen-stablecoin)) | Live | All yen stablecoins together about $236 million |
| **Korean won stablecoins** | Legislation under debate | Mostly not live | Under $1 million |
| **Bank-issued tokens** | Deposit tokens from banks | Pilots | About $0.24 billion in total |

*Market caps from CoinGecko, November 8, 2026.*

**The lesson:** announcements from large companies are treated as competition years before they carry payments. The library tracks use, not press releases.

## Who wants dollars, and who doesn't

**People who want dollars** live where the local currency is losing value or can't be trusted. A BIS working paper (March 2026) found over 70% of net stablecoin inflows came from non-dollar currencies, rising as local currencies weakened. Flows reached about 7–8% of GDP in parts of Latin America, the Caribbean, Africa and the Middle East (LSE Business Review, May 2026) ([Shaping Tomorrow summary](https://decision-intel.shapingtomorrow.com/scans/financial-services-future-of-money/2026-06-08-invisible-dollarisation/scan.html)). The earlier scans show the same in Argentina, Nigeria, Bolivia, Iran and Lebanon.

**Most people don't want dollars.** For anyone whose salary, rent and prices are in a stable currency (euros, yen, won, pounds, Swiss francs), holding dollars *adds* risk: their money moves against the euro or the yen. "Stable" means stable in *their* currency. That's why:

- **Non-dollar stablecoins are small but growing as working money.** A Visa and Dune report found non-dollar stablecoin supply reached $1.1 billion in February 2026, about three times its January 2023 level, with transfer volume up over 1,600% to $10 billion. Euro stablecoins are over 80% of that, Brazilian real about 10%. The authors describe them as "operational money for cross-border payments, remittances, B2B settlement, and FX management" ([The Block](https://www.theblock.co/post/395038/beyond-dollarization-visa-and-dune-report-finds-non-usd-stablecoins-increasingly-being-used-as-money)).
- **Governments are pushing back on dollar tokens.** The ECB's Isabel Schnabel warned in June 2026 that dollar stablecoins endanger monetary sovereignty in economies with weaker monetary credibility. China and several Gulf states have banned them; Japan chose licensed domestic stablecoins; the UK an authorization regime ([Shaping Tomorrow summary](https://decision-intel.shapingtomorrow.com/scans/financial-services-future-of-money/2026-06-08-invisible-dollarisation/scan.html)); Brazil banned stablecoin settlement in cross-border payments ([CoinDesk](https://www.coindesk.com/policy/2026/05/02/brazil-s-central-bank-bans-stablecoin-and-crypto-settlement-in-cross-border-payments)).
- **Some people want neither dollars nor bitcoin:** tokenized gold is about $5.1 billion, larger than all non-dollar stablecoins combined.

**For this library:** a K-pop group order priced in won, otoshidama in yen or a Berlin club collective's kitty in euros doesn't need dollars at all. Outside dollarizing economies, the question isn't "bitcoin or stablecoins" but **"how do people think and price in their own currency while bitcoin moves underneath?"**

## Properties compared with bitcoin

| | Company-issued dollar stablecoin | Bitcoin |
| --- | --- | --- |
| **Issuer** | A company (or consortium) | None |
| **Can be frozen** | Yes, by the issuer | No |
| **Value** | Stable in dollars; moves against other currencies | Volatile in every currency |
| **Yield** | US law (GENIUS Act, signed July 18, 2025) bars issuers from paying holders for holding; whether third parties can pass on "rewards" is still debated ([Spark research](https://www.spark.money/research/stablecoin-yield-prohibition-debate)). Open USD shares reserve income with businesses. | None |
| **Self-custody** | Possible, but the issuer can still freeze | Full |
| **Privacy** | Public on most chains; issuers and exchanges see identities | Varies by layer (on-chain public; Lightning and Ark more private) |
| **Regulation** | Licensing regimes (GENIUS, MiCA, Japan, UK) | Mostly treated as an asset |
| **Rails** | Many chains: Tron, Ethereum, Solana, Tempo and more | Bitcoin, Lightning, Ark, Liquid and others |

## Stablecoins on bitcoin

- **Lightning:** USDT through Taproot Assets has been live since March 2026, still nascent ([Spark research](https://spark.money/research/lightning-network-2026-state)).
- **Ark:** Tether backed Ark Labs' seed round to bring stablecoins to Arkade ([The Block](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin)). Second hasn't announced stablecoin plans for Bark. *[to verify]*
- **Other bitcoin layers:** Spark, Liquid and RGB support or plan dollar tokens *[from memory; to verify]*.
- **Synthetic bitcoin-based dollars:** Blink's Stablesats ([Blink](https://blink.sv/en/dollar-balance)).
- **Swaps instead of holding:** atomic swaps between Lightning and USDT ([Bitcoin Magazine on Boltz](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users)).

"Bitcoin versus stablecoins" is partly a false choice: the same rails can carry both.

## What it means for the research areas

| Area | What changes |
| --- | --- |
| 11 Community-driven economies | Most of these communities price in their own currency (won, yen, euros). Local-currency pricing and conversion matter more than dollars. |
| 12 Earning in bitcoin | Dollar stablecoins win where earners want dollar income, mostly in weak-currency economies. Elsewhere, earners want their own currency. |
| 13 Agentic payments | Agent payments are dollar-denominated (USDC on x402) by default. |
| 14 Dollars and bitcoin | The real competitor is specific: USDT on Tron in emerging markets. The stance question widens from "dollars" to "the user's own currency." |
| 15 Money that can't be frozen | Freezes are an issuer property; the argument for bitcoin is strongest against company-issued tokens. |
| 18 Last-mile infrastructure | Swaps should reach local currencies and local stablecoins (euro, real, yen), not only USDT. |

## Open questions

1. How much of the $350–550 billion in stablecoin payments is cross-border, and in which corridors?
2. Who actually uses non-dollar stablecoins, and for what?
3. Will Open USD's revenue sharing with businesses pull distribution away from USDT and USDC, and does it touch emerging markets at all?
4. Does Tempo carry real payment volume yet?
5. In stable-currency countries, do people want a stable token at all, or just good local payment apps?

## Sources

- [CoinGecko stablecoin categories and markets](https://www.coingecko.com/en/categories/stablecoins) (retrieved November 8, 2026)
- [Finextra on a16z's State of Crypto 2025](https://www.finextra.com/blogposting/29723/deep-dive-what-a16zs-state-of-crypto-2025-really-says-about-stablecoins-and-ai)
- [DigitalToday on stablecoins becoming local](https://www.digitaltoday.co.kr/en/view/51250/stablecoins-share-of-local-payments-rises-as-cross-border-use-fades)
- [Yahoo Finance on the Artemis report](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html)
- [ForkLog on Tron's falling share](https://forklog.com/en/trons-share-in-stablecoin-transactions-plummets-to-14/)
- [DEV Community on Tempo's launch](https://dev.to/tomwangcn/stripe-tempo-goes-live-ai-agent-payment-rails-3306)
- [The Block on Open USD](https://theblock.co/post/406736/visa-stripe-coinbase-join-open-usd-stablecoin-shares-reserve-revenue)
- [Unlock on JPYC's launch](https://unlock-bc.com/en/japan-launches-worlds-first-regulated-yen-stablecoin)
- [The Block on the Visa and Dune non-dollar stablecoin report](https://www.theblock.co/post/395038/beyond-dollarization-visa-and-dune-report-finds-non-usd-stablecoins-increasingly-being-used-as-money)
- [Shaping Tomorrow on "invisible dollarisation"](https://decision-intel.shapingtomorrow.com/scans/financial-services-future-of-money/2026-06-08-invisible-dollarisation/scan.html)
- [CoinDesk on Brazil's settlement ban](https://www.coindesk.com/policy/2026/05/02/brazil-s-central-bank-bans-stablecoin-and-crypto-settlement-in-cross-border-payments)
- [Spark research on the stablecoin yield debate](https://www.spark.money/research/stablecoin-yield-prohibition-debate)
- [Spark: State of the Lightning Network in 2026](https://spark.money/research/lightning-network-2026-state)
- [The Block on Tether backing Ark Labs](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin)
- [Blink Dollar Balance](https://blink.sv/en/dollar-balance)
- [Bitcoin Magazine on Boltz USDT swaps](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users)
