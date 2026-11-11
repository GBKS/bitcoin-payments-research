# Dollars and bitcoin

*Deep dive, first draft. Builds on the November 9 quick scan and its claims check. Desk research only. Last updated November 11, 2026.*

## Thesis

Stablecoins are winning payments. Bitcoin builders hear it from merchants directly; merchants told one builder to "support USDT or go away" ([quoted by Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)). The evidence below suggests what they're asking for:

- **Stable value in the money their counterparties already use,** and a way around banks that have no dollars or slow foreign exchange. Not USDT as such.
- **Settlement, more than holding.** In the trade flows that are best documented, USDT passes between brokers for an hour; the supplier at the other end receives local currency.
- **Another issuer when one fails, not bitcoin.** When people lost trust in a stablecoin or faced freezes, the observed move was to a different stablecoin.

At the same time, the places where bitcoin and dollars already meet mostly settle in dollars: Square's merchants receive dollars by default, and a merchant showcased by Blink converts every payment to her dollar balance.

**The hypothesis:** for bitcoin wallets, the dollar question is mostly about the edges: showing prices in the user's currency, locking rates, and swapping at the moment of payment. Holding dollars inside a bitcoin wallet is a second, harder question, and the dollar rails on bitcoin that would make it self-custodial are still early.

*Status: a working hypothesis from desk research. Nobody has asked the merchants who say "support USDT" what would make them accept something else; that's the first gap direct research would fill.*

## What we mean

**Dollars** here means dollar stablecoins, mostly USDT, plus bitcoin-based synthetic dollars. [Stablecoins, unpacked](03-stablecoins.md) explains the kinds and why most people outside dollarizing economies want stability in their own currency, not dollars.

**Four stances a bitcoin wallet can take,** from purest to most flexible:

| Stance | What the user holds | What it takes |
| --- | --- | --- |
| 1. Bitcoin only | Bitcoin, shown in sats or ₿ | Nothing extra |
| 2. Local-currency display | Bitcoin, shown in local currency, with rates locked when an order or invoice is created | A price feed |
| 3. Swaps at the edges | Bitcoin; pays people who want stablecoins, or gets paid by people who only have them | A swap service at the moment of payment |
| 4. A dollar balance | Dollars next to bitcoin, on a bitcoin layer or through a service | A dollar rail, an issuer, often a provider |

The design problem is real at every step: two currencies in one wallet, without confusing people about what they hold.

## What people say, and what they do

**Say:**

- In a Visa-sponsored survey by Castle Island and Brevan Howard of about 2,500 crypto users in Nigeria, Turkey, Brazil, India and Indonesia, the main uses beyond trading were currency conversion, paying for goods, remittances and salaries. Nigerians most wanted to save in dollars; an Indonesian exchange said stablecoins are easier to get than a dollar bank account ([The Block](https://www.theblock.co/post/316048/survey-visa-brevan-howard-castle-island-ventures-stablecoins-real-world-application), September 2024).
- In a BVNK and YouGov survey of 4,658 current or prospective crypto holders in 15 countries, the top reasons were lower fees and faster cross-border transfers ([Cointelegraph](https://cointelegraph.com/news/bvnk-survey-finds-growing-use-of-stablecoins-for-income-and-everyday-payments), February 2026). *BVNK sells stablecoin infrastructure.*
- Bolivian small-business owners cite banks with no dollars and a falling boliviano ([Jakarta Post / Reuters](https://www.thejakartapost.com/business/2025/06/26/crypto-gains-foothold-in-bolivia-as-small-businesses-seek-currency-alternatives), June 2025).

**Do:**

- **USDT on Tron is the default for stablecoin payments.** Artemis studied 31 stablecoin payment companies, a snapshot annualizing to $72.3 billion across business, peer-to-peer, consumer and card payments. USDT was 90% of payment volume, and Tron carried about 60% ([Yahoo Finance](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html), May 2025). Dragonfly's Rob Hadick said payment firms care little which chain settles, since Tron is fast and cheap, and that Tether is a trusted brand in places like Argentina and Brazil, where people worry about bank failures.
- **Income too:** stablecoins were over 90% of crypto salaries in 2024 ([Earning in bitcoin](12-earning-in-bitcoin.md)).
- **People buy dollars and hold bitcoin.** On Bitso in Argentina in the first half of 2025, stablecoins were 85% of purchases and bitcoin 4%, yet bitcoin was in 55% of wallets ([iProfesional](https://www.iprofesional.com/tecnologia/435197-argentinos-eligen-el-dolar-digital-para-el-dia-a-dia-y-bitcoin-para-el-largo-plazo)). Across Bitso's four Latin American markets in 2025, bitcoin was 18% of purchases but 52% of portfolios by value ([Bitso](https://bitso.com/blog/crypto-landscape-in-latin-america-2025/), April 2026). *Exchange data; bitcoin's price rise inflates its share of holdings.*
- **Fewer people use stablecoins for purchases than say they want to:** 42% of BVNK's respondents want to use them for major purchases; 28% do ([Cointelegraph](https://cointelegraph.com/news/bvnk-survey-finds-growing-use-of-stablecoins-for-income-and-everyday-payments)).

**Say versus do:** merchants *say* "support USDT." What they *do* is settle in USDT on Tron, mostly through payment companies, without caring much about the chain. That suggests they want *stable dollars their counterparties already use*, not USDT as such.

## Why existing options serve them badly

Both sides fall short, in different ways.

**Stablecoins:**

- **They can be, and are, frozen.** Tether froze more than $514 million in USDT across 370 addresses in the 30 days before May 8, 2026, about 98% of it on Tron. In 2025, 4,163 addresses were blacklisted with $1.26 billion frozen ([Cointelegraph on BlockSec data](https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show)). By July 2026, BlockSec counted 9,597 blacklisted USDT addresses on Ethereum and Tron holding about $5.69 billion ([BlockSec](https://blocksec.com/blog/usdt-blacklist-explained-2026)). Most freezes target illicit activity, but the power is the issuer's.
- **The law requires the power to freeze.** The US GENIUS Act requires a permitted issuer to have "the technological capability to comply" with lawful orders, including orders to freeze, burn or prevent transfers ([GENIUS Act](https://www.govinfo.gov/content/pkg/BILLS-119s1582enr/html/BILLS-119s1582enr.htm), signed July 18, 2025).
- **Legitimate businesses get caught.** In March 2026 Circle froze USDC in 16 business wallets linked to a sealed civil case, and unfroze one after a public backlash ([The Block](https://www.theblock.co/post/395190/circle-unfreezes-usdc)).
- **Rules tighten country by country.** Brazil treats stablecoin purchases and transfers as foreign exchange, requires a license, and requires providers to identify the owner of any self-custody wallet they send to or receive from ([Cointelegraph](https://cointelegraph.com/news/brazil-central-bank-crypto-rules-stablecoins-foreign-exchange), November 2025). Turkey caps stablecoin withdrawals from platforms at $3,000 a day and $50,000 a month ([Legal 500](https://www.legal500.com/intelligence/turkey/technology/masak-communique-introducing-tightened-measures-for-crypto-asset-service-providers-has-entered-into-force), 2025).

**Bitcoin wallets:**

- **Volatility** for anyone pricing, saving or restocking in dollars.
- **Swaps are taxable.** Swapping bitcoin for a stablecoin is a disposal in the US ([IRS](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions), Q16), the UK ([HMRC](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto22100)) and Germany, where it also restarts the one-year holding period ([BMF letter](https://www.deubner-steuern.de/fileadmin/media/Steuern/downloads/files/kryptowerte_bmf_2025-03-06.pdf), March 2025). A wallet that swaps at every payment creates a tax record at every payment.
- **Dollar rails on bitcoin are early** (below), so a self-custodial dollar balance mostly isn't available yet.

## Case studies

### Lagos to Guangzhou: USDT as a settlement rail

Electronics traders in Lagos's Computer Village pay suppliers in Guangzhou in under an hour. A broker converts naira to USDT on peer-to-peer platforms; Chinese crypto traders convert the USDT to yuan and pay the supplier through Chinese banks, so the supplier never touches crypto. The official foreign-exchange route took 7 to 21 days with no guarantee of approval. Brokers carry the fraud risk ([Down To Earth, via The Conversation](https://www.downtoearth.org.in/africa/nigerias-crypto-boom-isnt-just-about-technology-trust-plays-a-role-in-the-local-gadget-trade-with-china), March 2026).

**What it shows:** "the supplier wants USDT" may really mean "the broker settles in USDT." Merchants want speed and certainty; the rail is invisible to them.

### Bolivia and Venezuela: dollars when banks have none

- **Bolivia.** Car dealers for Toyota, Yamaha and BYD accept USDT because of the dollar shortage ([Cointelegraph](https://cointelegraph.com/news/toyota-and-yamaha-accept-usdt-bolivia-as-usd-reserves-fall), September 2025). A duty-free shop prices goods in USDT but still accepts bolivianos and dollars ([Cointelegraph](https://cointelegraph.com/news/tether-usdt-prices-goods-bolivia), June 2025). A former central bank head estimated USDT volume at about $600,000 a day, against $18–22 million in the formal market ([Jakarta Post / Reuters](https://www.thejakartapost.com/business/2025/06/26/crypto-gains-foothold-in-bolivia-as-small-businesses-seek-currency-alternatives)). Some businesses also accept bitcoin.
- **Venezuela.** An estimated 1.389 billion USDT traded on Binance's peer-to-peer market in about a month in mid-2026, around 44 million a day, equal to 88% of the central bank's foreign-currency sales ([Bitcoin.com News, citing Ecoanalítica](https://news.bitcoin.com/latam-insights-unpacking-bolivias-stablecoin-push-venezuelas-massive-p2p-market-and-argentinas-libra-crackdown/), July 2026). Shops price in dollars and settle at the peer-to-peer rate ([DigitalToday](https://www.digitaltoday.co.kr/en/view/72475/venezuela-p2p-market-usdt-price-up-16-percent-in-a-month), June 2026).

**What it shows:** USDT works as a parallel foreign-exchange market. In Venezuela it's a primary channel; in Bolivia it's still small next to the formal market.

### When trust in an issuer breaks

- **USDC, March 2023.** When USDC lost its peg, the dominant movement among 1,359 active accounts studied was from USDC to USDT ([arXiv](https://arxiv.org/html/2606.07442v1), 2026). *Mostly DeFi users, not emerging-market merchants.*
- **Iran, 2025.** After Tether froze 42 addresses in July 2025, Iranian exchanges and channels urged users to move from USDT on Tron to DAI on Polygon ([Coinlive, citing TRM Labs](https://www.coinlive.com/news/iran-s-crypto-scene-takes-a-11-hit-after-nobitex-hack)). During protests in early 2026, withdrawals of *bitcoin* from Iranian exchanges to personal wallets rose sharply, "possibly as a flight to safety" ([The Block, citing Chainalysis](https://www.theblock.co/amp/post/385941/iran-crypto-ecosystem-irgc-footprint-bitcoin-withdrawals-surge-during-protests-chainalysis), January 2026).

**What it shows:** for payments, people swap issuers. Bitcoin shows up as a refuge for savings under stress, not as the payment replacement. See [Money that can't be frozen](15-money-that-cant-be-frozen.md).

### Bitcoin meets dollars at the counter

- **Square.** About 1 million US merchants are enabled to accept bitcoin over Lightning since Square switched it on by default on March 30, 2026. Merchants receive dollars by default ([Bitcoin Magazine](https://bitcoinmagazine.com/news/square-crosses-1-million-bitcoin-merchants), May 2026). *"Enabled" counts merchants who didn't opt out; no usage figures are published.*
- **A Blink merchant in Nigeria** converts each payment she receives into her dollar balance to restock ([Blink](https://www.blink.sv/blog/the-practical-power-of-stablesats-in-a-bitcoin-circular-economy), May 2026). *Vendor content.*

**What it shows:** where bitcoin acceptance meets everyday costs, merchants settle in dollars. The payer can still pay in bitcoin.

### Bitcoin wallets that added dollars

| Wallet | How the dollars work | Custody | Since |
| --- | --- | --- | --- |
| Blink | Dollar Balance: Stablesats (a synthetic dollar held through derivatives) in custodial mode; USDB, a stablecoin issued by Brale on Spark, in non-custodial mode | Both | Stablesats 2022; non-custodial accounts June 2026 |
| Wallets on the Breez SDK (Glow, Blitz) | "Stable balance": received sats convert to USDB above a threshold, and back to sats when paying | Self-custodial | 2026 |
| Wallet of Satoshi | Stablecoins in its new version, reportedly USDB on Spark | Disputed in reports | Beta July 2026, switched on September |
| Speed | USDT on Lightning through Taproot Assets | Custodial bridge | *[to verify: no source gives a date; USDT on Lightning went live in March 2026]* |
| Aqua | USDT on Liquid next to bitcoin, Liquid and Lightning | Self-custodial | 2023 *[from memory]* |

- Blink offers a Dollar Balance, custodial through Stablesats or non-custodial with supported stablecoins ([Blink](https://www.blink.sv/en/dollar-balance)); in non-custodial mode it holds USDB on Spark ([Blink FAQ](https://faq.blink.sv/llms-full.txt)), and Blink calls Spark "trust-minimized, not trustless" ([Blink](https://blink.sv/blog/non-custodial-accounts-in-blink-wallet), June 2026).
- The Breez SDK offers a "stable balance" that converts received sats to a stablecoin ([Breez SDK docs](https://sdk-doc-spark.breez.technology/guide/stable_balance.html)), with Glow as an open-source reference app ([Bitcoin Magazine](https://bitcoinmagazine.com/business/breez-announces-glow-an-open-source-bitcoin-to-stablecoins-progressive-web-app), August 2026) and Blitz letting users receive Lightning payments into either balance ([Value the Markets](https://www.valuethemarkets.com/cryptocurrency/news/blitz-wallet-update-making-bitcoin-more-like-money), May 2026).
- Wallet of Satoshi added stablecoins to its self-custodial version, in beta from July 2026 and switched on in September, according to secondary reports ([Coin-Turk](https://en.coin-turk.com/wallet-of-satoshi-launches-stablecoins-on-lightning-with-self-custody-option/), [Stacker News](https://stacker.news/items/1561905)). Another report names the stablecoin as USDB and calls the setup delegated custody ([CriptoNoticias](https://www.criptonoticias.com/mercados/seguridad-financiera-usdb-stablecoin-wallet-satoshi/), July 2026). *[to verify: official Wallet of Satoshi announcement]*
- Tether led an $8 million round in Speed, which reports 1.2 million users and over $1.5 billion in annual volume, not split by asset ([Cointelegraph](https://cointelegraph.com/news/tether-invests-bitcoin-stablecoin-startup-speed1), December 2025).
- In September 2026, attackers drained about 4,000 BTC (about $320 million) from Liquid's federation wallet through a software bug, and Liquid paused; Liquid said USDT on Liquid was unaffected ([Cointelegraph](https://cointelegraph.com/news/liquid-network-pauses-320m-bitcoin-withdrawal)). That matters for every wallet whose dollars or bitcoin sit on Liquid.

**Design patterns:** Blink shows bitcoin and dollar accounts side by side with local-currency equivalents, lets users make the dollar account the default so bitcoin payments land as dollars, and charges a 0.2% spread to convert ([Blink](https://blink.sv/blog/blink-wallet-just-got-better), [Blink](https://blink.sv/blog/navigating-the-blink-convert-feature-easily-convert-between-your-bitcoin-and-dollar-account)). The Breez SDK converts automatically and asks apps to show conversion status (pending, completed, failed, refunded) ([Breez SDK docs](https://sdk-doc-spark.breez.technology/guide/stable_balance.html)).

**What it shows:** no wallet publishes how many users hold dollars, how much, or whether people move from dollars into bitcoin over time. The claim that a dollar balance is an on-ramp to bitcoin is untested. And the rail under a dollar balance can change without the user noticing: Blink's moved from Stablesats to USDB.

## Dollar rails on bitcoin

| Rail | Status, November 2026 | Size | Who can freeze or control |
| --- | --- | --- | --- |
| USDT on Lightning (Taproot Assets) | Tether announced USDT on bitcoin and Lightning through Taproot Assets in January 2025 ([The Block](https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership)). It went live in March 2026 according to secondary reports ([Live Bitcoin News](https://www.livebitcoinnews.com/tether-usdt-lands-on-bitcoins-lightning-network/)); the ecosystem is "still nascent," mostly LND-based, with early adoption through Speed Wallet and LnFi, and the report gives no volumes ([Spark research](https://spark.money/research/lightning-network-2026-state)). Lightning Labs' own Wavelength still listed stablecoins as "coming soon" in October 2026 ([Lightning Labs](https://lightning.engineering/blog/)). | Not published | Edge nodes that convert need USDT inventory and bitcoin liquidity ([Lightning Labs docs](https://docs.lightning.engineering/the-lightning-network/taproot-assets/edge-nodes)); issuer freezing *[to verify]* |
| USDT on Liquid | Live since 2019; Liquid paused after the September 2026 exploit | About $97.6 million issued, of which about $63.8 million is held in reserve, so roughly $34 million in circulation ([Tether](https://app.tether.to/transparency.json), November 10, 2026) *[the subtraction is ours]* | Tether; Liquid's federation |
| USDB on Spark | Live since January 2026; issued by Brale, with rewards paid in bitcoin ([Spark](https://www.spark.money/news/usdb-rewards-stablecoin)) | Not published | The issuer can ask Spark's operators to freeze; "not enforced at the protocol level" ([Spark docs](https://docs.spark.money/learn/tokens/freezing)) |
| Stablecoins on Arkade (Ark) | Tether backed Ark Labs' $5.2 million seed round in March 2026 to expand stablecoin support on Arkade, the other main Ark implementation ([The Block](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin)). Tether hadn't committed to issuing USDT there ([Decrypt](https://decrypt.co/360773/tether-backs-ark-labs-bet-on-bitcoins-stablecoin-revival)). | No live USDT found | Whoever holds the control asset can increase supply ([Arkade docs](https://docs.arkadeos.com/learn/arkade-assets/overview.md)) |
| Bark (Ark, by Second) | Launched on mainnet in June 2026 for "self-custodial bitcoin payments" ([Bitcoin Magazine](https://bitcoinmagazine.com/news/second-launches-bark-on-bitcoin-mainnet)). As of November 2026, Second hasn't announced plans for stablecoins in Bark. *[to verify]* | Bitcoin only | — |
| USDT on RGB | Not live; Utexo, backed by Tether, plans a public launch on November 28, 2026, with Lightning in early 2027 ([Bitcoin Magazine](https://bitcoinmagazine.com/news/utexo-opens-early-access-to-usdt-on-bitcoin-through-utexo-mint)) | — | Backed by Tether's USDT0 |
| Rootstock | Live: USDT0, DOC, USDRIF and others | About $8.8 million in stablecoins in total ([DefiLlama](https://stablecoins.llama.fi/stablecoins), November 10, 2026) | Varies by token |
| Synthetic (Stablesats) | Live in Blink's custodial mode | Not published | The service |

**Swaps instead of holding:** Boltz launched non-custodial swaps from Lightning to USDT in March 2026, routed through Arbitrum ([Bitcoin Magazine](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users)). Those swaps were disabled on August 1, 2026, and on August 3 Boltz suspended all swaps "until further notice," citing AI-assisted attacks; no user funds were lost ([Bitcoin News](https://bitcoinnews.com/p/boltz-suspends-bitcoin-services-ai-assisted-attacks)). FixedFloat charges 0.5–1% plus network fees ([FixedFloat](https://ff.io/faq)). A draft standard for wallets to discover swap providers, SSPS, covers Lightning, Liquid, Arkade, Bark and RGB but not Spark or Taproot Assets, and lists no adopters yet ([SSPS](https://github.com/kaleidoswap/ssps)). See [Last-mile infrastructure](18-last-mile-infrastructure.md).

**Interoperability:** dollars on different bitcoin layers don't move directly between each other. Getting from one to another means swapping through bitcoin or through a service. Several of the new rails are backed by Tether's USDT0, which in principle connects to USDT on Tron through Tether's own bridges ([CryptoSlate](https://cryptoslate.com/tether-introduces-bridge-free-multichain-liquidity-for-legacy-usdt-networks/)).

*Several rail descriptions come from Spark's research and comparison pages; Spark builds a competing layer.*

## Lessons from elsewhere

How people live with two currencies, from multi-currency accounts, dual-currency economies, loyalty points and games:

- **Separate balances, explicit conversion.** Wise lets customers hold "as many different currencies" as they like in separate balances, converted at the mid-market rate ([Wise](https://wise.com/help/articles/2897226/what-are-balances)). No published research says whether this confuses people.
- **Each currency gets a role.** In Cambodia, the riel "is used only for small transactions worth less than about five dollars in urban areas," and change from dollar payments is given in riel ([JICA](https://www.jica.go.jp/english/jica_ri/news/interview/2013/jica-ri_focus_vol26.html), 2014). Lebanese supermarkets switched to dollar prices to stop price manipulation and display the exchange rate, with a time stamp, next to the price ([The National](https://www.thenationalnews.com/mena/lebanon/2023/03/01/dollars-or-pounds-lebanons-supermarkets-begin-pricing-goods-in-dollars), 2023). Zimbabwe requires shops to show prices in both currencies ([Insider Zimbabwe](https://insiderzim.com/why-zimbabwe-requires-businesses-to-display-prices-in-zim-and-us-dollars/), 2020). Showing two currencies is normal; the question is which one sets the price.
- **A second unit gets hoarded, and distrusted when it changes value.** About a third of US loyalty rewards go unredeemed ([Advanced Management on Stourm et al.](https://advancedmanagement.net/perspectives/2017/08/why-consumers-stockpile-rather-spend-loyalty-program-points)), and US regulators are investigating airlines for devaluing earned points ([AirlineGeeks](https://airlinegeeks.com/2024/09/06/dot-probe-investigates-four-largest-airline-rewards-programs/), 2024).
- **Regulators want the real price visible.** EU consumer authorities' 2025 principles say the price of in-game content "should be clearly indicated in real-world money," and traders "should not obscure the cost" ([Linklaters](https://techinsights.linklaters.com/post/102k6t4/game-changer-eu-introduces-consumer-protection-guidance-for-in-game-virtual-curr)). Cryptocurrencies are out of their scope, but the principle of showing a local-currency equivalent next to a bitcoin amount points the same way.

## Sizing

| Flow | Size | Source |
| --- | --- | --- |
| USDT on Tron, issued | about $94.2 billion | [Tether](https://app.tether.to/transparency.json), November 10, 2026 |
| Stablecoin payment companies studied by Artemis | about $72.3 billion a year | [Yahoo Finance](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html) |
| Venezuela's peer-to-peer USDT market | about 44 million USDT a day, mid-2026 | [Bitcoin.com News](https://news.bitcoin.com/latam-insights-unpacking-bolivias-stablecoin-push-venezuelas-massive-p2p-market-and-argentinas-libra-crackdown/) |
| Bolivia's USDT market | about $600,000 a day, 2025 | [Jakarta Post / Reuters](https://www.thejakartapost.com/business/2025/06/26/crypto-gains-foothold-in-bolivia-as-small-businesses-seek-currency-alternatives) |
| USDT on Liquid, in circulation | roughly $34 million | [Tether](https://app.tether.to/transparency.json) |
| All stablecoins on Rootstock | about $8.8 million | [DefiLlama](https://stablecoins.llama.fi/stablecoins) |
| USDT on Lightning, USDB on Spark | Not published | |

The dollars on bitcoin layers that can be counted, about $43 million, are less than a two-thousandth of USDT on Tron. Lightning's share of stablecoin volume was "near zero" in 2025, by a Lightning infrastructure company's own account ([Cointelegraph](https://cointelegraph.com/interview/lightning-network-5-percent-stablecoin-volume-voltage-ceo)).

## Key assumptions

1. **Merchants want stable value and their counterparties' currency, not USDT itself.** Supported by the Lagos chain and Bolivian pricing. Contradicted if merchants turn down other stable dollars that settle as fast.
2. **Settling at the edges is enough for most merchants.** Supported by Square's defaults and the Blink merchant. Contradicted if merchants need to *hold* dollars for weeks, as savers do.
3. **Self-custodial dollars on bitcoin will have liquidity.** Not yet supported: the countable rails are tiny and the largest ones publish no figures.
4. **A dollar balance leads people toward bitcoin.** Untested: no wallet publishes this.

## What could serve this

**Kinds of product**

- **Wallet stances** toward dollars (above).
- **Swap services** between bitcoin and stablecoins or local money (Boltz, suspended since August 2026; SSPS providers; [Last-mile infrastructure](18-last-mile-infrastructure.md)).
- **Merchant tools** that accept one currency and settle in another, as Square and Blink do.
- **Pricing tools:** displaying local currency and locking rates in invoices and orders.
- **Broker tools:** the people who connect local money to USDT and back, as in the Lagos chain, are few and central, like group order managers in [Community-driven economies](11-community-driven-economies.md).

## Trade-offs for self-custodial, client-side products

| Stance | Self-custody | Without your own server | Where it gets hard |
| --- | --- | --- | --- |
| Local-currency display and rate locks | Fully | Needs a price feed | Which rate to show; who honors a locked rate when the price moves |
| Swaps at the edges | Fully, with non-custodial swaps | Needs a swap provider | Fees and slippage, liquidity, and a taxable event at every swap |
| Dollar balance on a bitcoin layer | Partly: the user holds keys, but the issuer can freeze and operators or edge nodes are trusted | Needs the layer's operators | Rails are early; freeze powers return; balances may need regulated partners |
| Dollar balance through a provider | No | Needs the provider | Licensing and identity checks (GENIUS for custodial providers from about 2028, MiCA, Brazil, Turkey) |

**Where self-custody genuinely conflicts**

- **Freezes come back.** Any dollar token has an issuer, and US law requires the ability to freeze. Self-custody of the keys doesn't remove that.
- **Rules reach the other side.** The GENIUS Act excludes self-custodial software and direct transfers between individuals, but Brazil requires providers to identify who owns a self-custody wallet they deal with.
- **Two currencies, one mental model.** A wallet that converts automatically can leave people unsure what they hold, and every conversion is a tax record.

## Risks and open questions

**Risks**

- **Issuer risk:** stablecoins bring back an issuer who can freeze funds, which undercuts self-custody.
- **Regulation:** stablecoin rules (GENIUS Act in the US, Brazil's foreign-exchange rules, Turkey's caps) change quickly.
- **Immaturity:** dollar rails on bitcoin are early, with few wallets, little liquidity and, in Liquid's case, a recent exploit.
- **Identity:** for wallets built around bitcoin, adding dollars can blur what they stand for.

**Open questions**

1. When merchants ask for USDT, what do they need: stable value, their counterparties' currency, a dollar savings account, or simplicity?
2. Would swaps at the edges satisfy them, or do they need to *hold* dollars?
3. Do wallets that added dollars (Blink, Speed) see people move into bitcoin over time, or stay in dollars?
4. Which dollar rails on bitcoin will have liquidity in 2027: Taproot Assets, Spark, Arkade, RGB, or others? Can a bitcoin-only wallet swap with all of them at the edges?
5. Do brokers, rather than merchants, decide which stablecoin a trade flow uses?

## Research plan: say, do, make

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 10 merchants and 3 brokers who settle in USDT, in one corridor (for example Lagos–Guangzhou or Bolivia) | Why USDT, what else they'd accept, how long they hold it |
| Following payments | Do | 3–5 real supplier payments, end to end | Each conversion, fee, delay and party |
| Price and settlement logs | Do | Merchants who accept both bitcoin and dollars | How often they convert, and when |
| Workaround teardown | Make | Brokers' rate sheets, chats and spreadsheets | How rates, trust and disputes are managed |
| Wallet comparison | Do | Blink, Breez SDK wallets, Wallet of Satoshi, Aqua | How each presents two currencies; where test users get confused |

**Outputs:** a money-flow map of one corridor, a comparison of wallet stances, and an updated thesis.

*[Open: which corridor, language support for interviews, and how to recruit brokers without exposing them.]*

## Sources

**Context:** [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what) · [Stablecoins, unpacked](03-stablecoins.md)

**Say and do:** [The Block on the Castle Island survey](https://www.theblock.co/post/316048/survey-visa-brevan-howard-castle-island-ventures-stablecoins-real-world-application) · [Cointelegraph on the BVNK survey](https://cointelegraph.com/news/bvnk-survey-finds-growing-use-of-stablecoins-for-income-and-everyday-payments) · [Yahoo Finance on the Artemis report](https://finance.yahoo.com/news/tether-tron-dominate-fast-growing-140000492.html) · [iProfesional on Argentina](https://www.iprofesional.com/tecnologia/435197-argentinos-eligen-el-dolar-digital-para-el-dia-a-dia-y-bitcoin-para-el-largo-plazo) · [Bitso on Latin America](https://bitso.com/blog/crypto-landscape-in-latin-america-2025/)

**Issuer risk and rules:** [Cointelegraph on Tether freezes (BlockSec data)](https://cointelegraph.com/news/tether-freezes-over-500m-usdt-30-days-blocksec-data-show) · [BlockSec on the USDT blacklist](https://blocksec.com/blog/usdt-blacklist-explained-2026) · [The Block on Circle's freeze](https://www.theblock.co/post/395190/circle-unfreezes-usdc) · [GENIUS Act](https://www.govinfo.gov/content/pkg/BILLS-119s1582enr/html/BILLS-119s1582enr.htm) · [Cointelegraph on Brazil's rules](https://cointelegraph.com/news/brazil-central-bank-crypto-rules-stablecoins-foreign-exchange) · [Legal 500 on Turkey](https://www.legal500.com/intelligence/turkey/technology/masak-communique-introducing-tightened-measures-for-crypto-asset-service-providers-has-entered-into-force) · [IRS virtual currency FAQ](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions) · [HMRC Cryptoassets Manual](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto22100) · [BMF letter on crypto](https://www.deubner-steuern.de/fileadmin/media/Steuern/downloads/files/kryptowerte_bmf_2025-03-06.pdf)

**Case studies:** [Down To Earth on Lagos traders](https://www.downtoearth.org.in/africa/nigerias-crypto-boom-isnt-just-about-technology-trust-plays-a-role-in-the-local-gadget-trade-with-china) · [Jakarta Post on Bolivia](https://www.thejakartapost.com/business/2025/06/26/crypto-gains-foothold-in-bolivia-as-small-businesses-seek-currency-alternatives) · [Cointelegraph on Bolivian car dealers](https://cointelegraph.com/news/toyota-and-yamaha-accept-usdt-bolivia-as-usd-reserves-fall) · [Cointelegraph on USDT pricing in Bolivia](https://cointelegraph.com/news/tether-usdt-prices-goods-bolivia) · [Bitcoin.com News on Venezuela](https://news.bitcoin.com/latam-insights-unpacking-bolivias-stablecoin-push-venezuelas-massive-p2p-market-and-argentinas-libra-crackdown/) · [DigitalToday on Venezuela](https://www.digitaltoday.co.kr/en/view/72475/venezuela-p2p-market-usdt-price-up-16-percent-in-a-month) · [arXiv on the USDC depeg](https://arxiv.org/html/2606.07442v1) · [Coinlive on Iran](https://www.coinlive.com/news/iran-s-crypto-scene-takes-a-11-hit-after-nobitex-hack) · [The Block on Iran's bitcoin withdrawals](https://www.theblock.co/amp/post/385941/iran-crypto-ecosystem-irgc-footprint-bitcoin-withdrawals-surge-during-protests-chainalysis) · [Bitcoin Magazine on Square](https://bitcoinmagazine.com/news/square-crosses-1-million-bitcoin-merchants)

**Wallets:** [Blink Dollar Balance](https://www.blink.sv/en/dollar-balance) · [Blink FAQ](https://faq.blink.sv/llms-full.txt) · [Blink on non-custodial accounts](https://blink.sv/blog/non-custodial-accounts-in-blink-wallet) · [Blink's redesign](https://blink.sv/blog/blink-wallet-just-got-better) · [Blink on converting](https://blink.sv/blog/navigating-the-blink-convert-feature-easily-convert-between-your-bitcoin-and-dollar-account) · [Blink on Stablesats in a circular economy](https://www.blink.sv/blog/the-practical-power-of-stablesats-in-a-bitcoin-circular-economy) · [Breez SDK: Stable Balance](https://sdk-doc-spark.breez.technology/guide/stable_balance.html) · [Bitcoin Magazine on Glow](https://bitcoinmagazine.com/business/breez-announces-glow-an-open-source-bitcoin-to-stablecoins-progressive-web-app) · [Value the Markets on Blitz](https://www.valuethemarkets.com/cryptocurrency/news/blitz-wallet-update-making-bitcoin-more-like-money) · [Coin-Turk on Wallet of Satoshi stablecoins](https://en.coin-turk.com/wallet-of-satoshi-launches-stablecoins-on-lightning-with-self-custody-option/) · [Stacker News on Wallet of Satoshi enabling stablecoins](https://stacker.news/items/1561905) · [CriptoNoticias on Wallet of Satoshi and USDB](https://www.criptonoticias.com/mercados/seguridad-financiera-usdb-stablecoin-wallet-satoshi/) · [Cointelegraph on Tether and Speed](https://cointelegraph.com/news/tether-invests-bitcoin-stablecoin-startup-speed1) · [Cointelegraph on the Liquid exploit](https://cointelegraph.com/news/liquid-network-pauses-320m-bitcoin-withdrawal)

**Rails and swaps:** [The Block on USDT on Lightning](https://www.theblock.co/post/338109/tethers-usdt-stablecoin-returns-to-bitcoin-with-lightning-labs-partnership) · [Live Bitcoin News on the go-live](https://www.livebitcoinnews.com/tether-usdt-lands-on-bitcoins-lightning-network/) · [Spark: State of the Lightning Network in 2026](https://spark.money/research/lightning-network-2026-state) · [Lightning Labs blog](https://lightning.engineering/blog/) · [Lightning Labs on edge nodes](https://docs.lightning.engineering/the-lightning-network/taproot-assets/edge-nodes) · [Tether transparency data](https://app.tether.to/transparency.json) · [Spark on USDB](https://www.spark.money/news/usdb-rewards-stablecoin) · [Spark docs on freezing](https://docs.spark.money/learn/tokens/freezing) · [The Block on Tether backing Ark Labs](https://www.theblock.co/post/393198/tether-backs-ark-labs-5-2-million-seed-raise-to-expand-stablecoin-and-programmable-finance-infrastructure-on-bitcoin) · [Decrypt on Ark Labs](https://decrypt.co/360773/tether-backs-ark-labs-bet-on-bitcoins-stablecoin-revival) · [Arkade docs on assets](https://docs.arkadeos.com/learn/arkade-assets/overview.md) · [Bitcoin Magazine on Bark](https://bitcoinmagazine.com/news/second-launches-bark-on-bitcoin-mainnet) · [Bitcoin Magazine on Utexo](https://bitcoinmagazine.com/news/utexo-opens-early-access-to-usdt-on-bitcoin-through-utexo-mint) · [DefiLlama stablecoins](https://stablecoins.llama.fi/stablecoins) · [Bitcoin Magazine on Boltz USDT swaps](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users) · [Bitcoin News on Boltz's suspension](https://bitcoinnews.com/p/boltz-suspends-bitcoin-services-ai-assisted-attacks) · [FixedFloat FAQ](https://ff.io/faq) · [SSPS](https://github.com/kaleidoswap/ssps) · [CryptoSlate on Tether's Legacy Mesh](https://cryptoslate.com/tether-introduces-bridge-free-multichain-liquidity-for-legacy-usdt-networks/) · [Cointelegraph interview on Lightning's stablecoin share](https://cointelegraph.com/interview/lightning-network-5-percent-stablecoin-volume-voltage-ceo)

*Research for this draft was done with AI agents, each claim checked against an opened source; the Liquid exploit, Square's merchant count, Lightning Labs' stablecoin status and Tether's Liquid figures were rechecked by hand. Claims carried over from the quick scan were checked in the [auto-research pilot](90-auto-research.md).*
