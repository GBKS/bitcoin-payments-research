# Where bitcoin is paid today

*Foundation document, first draft. A baseline of observed bitcoin payments, before asking where new demand could come from. Desk research only. Last updated November 11, 2026.*

## Why this page

The research areas start from where demand *might* come from. This page starts from the other end: where bitcoin is already paid, how much, and who asks for it. It also covers the uses bitcoin had and lost, and what the people who already hold bitcoin do with it. It puts the library's scattered sizing tables into one.

## The short version

- **The largest counted flow is Lightning, and much of it isn't payments.** About $1.17 billion moved over Lightning in November 2025, but the average transfer was $223 and exchange deposits and withdrawals are "a meaningful share." Nobody publishes the split.
- **At payment processors, bitcoin is one coin among several.** It was 22% of CoinGate's payments in 2025, and most merchants there settle in euros.
- **Bitcoin is paid where the recipient asks for it and has few other options:** gambling sites, darknet markets, ransomware, and privacy services. Even there it is losing share to stablecoins and Monero.
- **Bitcoin has lost payment uses.** Large merchants dropped it in 2017 and 2018 over fees, volatility and low demand; its share at processors has fallen since.
- **Most bitcoin doesn't move.** About 64% hasn't moved in a year, and about 3 million coins sit in ETFs, public companies and governments, where they can't be spent.
- **Holders who want to spend use dollars.** Crypto cards are funded mostly with stablecoins, and holders borrow against bitcoin instead of selling it.

## Sizes, side by side

*Rough annual figures in dollars, largest first. Sources and caveats are in the sections below or on the linked pages. Annualizing a single month is our arithmetic and overstates precision.*

| Flow | Size | What it measures |
| --- | --- | --- |
| Stablecoin payments, all rails | $350–550 billion a year | An estimate of actual payments ([Stablecoins, unpacked](03-stablecoins.md)) |
| Lightning, all transfers | $1.17 billion in November 2025, about $14 billion a year | Includes exchange deposits and withdrawals; share unknown |
| Crypto casinos | $10–81 billion a year in gross gaming revenue | All coins and some fiat; estimates disagree eightfold; bitcoin's share unknown |
| Crypto cards | $759 million in July 2026, about $9 billion a year | Tracked programs only; funded mostly with stablecoins |
| Darknet markets | about $2.5 billion in 2025 | Inflows Chainalysis can trace; excludes Monero |
| Ransomware | $820 million in 2025 | Extortion payments; mostly bitcoin |
| BitPay | "hundreds of millions of dollars" in 2025 | All coins; bitcoin's share not published |
| CoinGate | 1.42 million payments in 2025, 22% in bitcoin | Counts only; no value published |
| Remittances to El Salvador by crypto wallet | $57.7 million in 2025 | All crypto, not only bitcoin |
| Namecheap, bitcoin payments | $73 million over four and a half years, about $16 million a year | One merchant |
| x402 agent payments | about $15 million, lifetime to April 2026 | Almost all USDC ([Agentic payments](13-agentic-payments.md)) |
| Bitcoin Miner game payouts | over $3.7 million, lifetime | Company claim ([Earning in bitcoin](12-earning-in-bitcoin.md)) |
| Nostr zaps | 43 BTC, all time to August 2026 | One tracker ([Earning in bitcoin](12-earning-in-bitcoin.md)) |
| MoneyBadger, South Africa | about $1 million a year (2025) | Lightning at retail tills ([Last-mile infrastructure](18-last-mile-infrastructure.md)) |
| Fountain, listeners to podcasters | $127,900 in 2024 | ([Earning in bitcoin](12-earning-in-bitcoin.md)) |
| Square sellers, bitcoin payments | Not published | About 1 million merchants enabled ([Landscape](02-landscape.md)) |

**What it shows:** the flows this library studies most closely (zaps, podcasting, circular economies, agent payments) are the smallest rows. The large rows are transfers between exchanges, gambling, illicit markets and dollar-funded cards.

## Lightning: what the $1.17 billion is

- **The figure.** River estimates $1.17 billion and 5.22 million transactions over Lightning in November 2025; "The Lightning Network surpassed $1 billion in monthly volume, and grew by 300% in 2025" ([River](https://river.com/content/bitcoin-adoption-2026), February 2026). The estimate comes from 11 data providers covering about half of the network's capacity, scaled up ([River's report](https://river.com/learn/files/river-bitcoin-adoption-report-2026.pdf)). *River sells Lightning services. [to verify: the report's figures were read from page images, not text]*
- **Bigger transfers, not more of them.** In August 2023 River counted 6.6 million transactions worth $78.2 million, an average of $11.84 ([River, 2023](https://river.com/learn/files/river-lightning-report-2023.pdf)). By November 2025 there were fewer transactions and "The average transaction over the Lightning Network reached $223" ([River](https://river.com/content/bitcoin-adoption-2026)).
- **Exchanges explain the change.** In 2023 River thought it "unlikely that exchange withdrawals and deposits have been responsible for significant growth"; activity then was "gaming, social media tipping, and streaming." The 2026 report says exchange deposits and withdrawals "now make up a meaningful share of activity, pushing the average transaction size significantly higher." It gives no percentage.
- **Exchanges' own figures.** Coinbase said 15% of its bitcoin transactions moved over Lightning ([Lightspark](https://www.lightspark.com/blog/news/coinbase-lightning-network-lightspark), April 2025). Block said one in four of its outbound bitcoin payments went over Lightning ([CoinDesk](https://www.coindesk.com/tech/2025/05/29/square-flies-the-flag-for-the-lightning-network-with-97-yield-on-bitcoin-holdings), May 2025). Both are transfers, not purchases.

**What it shows:** Lightning's growth since 2023 is mostly people moving bitcoin between exchanges and wallets. The small payments that dominated in 2023 shrank in count. Lightning volume is a measure of reach, not of buying things.

## Payment processors

| Processor | Scale | Bitcoin's share | Settlement |
| --- | --- | --- | --- |
| CoinGate, 2025 | 1.42 million payments | 22.1%, the most-used coin; 11.3% of those over Lightning; stablecoins 29.8% | 62.5% to fiat, 25.2% to stablecoins |
| CoinGate, 2024 | 1.68 million payments | 22.8%, down from 35.6% in 2023; stablecoins 35.5% | 71% to euros, 8% kept in bitcoin |
| BitPay, 2025 | "nearly a million transactions," average $800 | Listed first by volume, no percentage; stablecoins 40% of volume | Not published |

Sources: [CoinGate 2025](https://coingate.com/blog/post/crypto-payments-data-report-2025), [CoinGate 2024](https://coingate.com/blog/post/crypto-payments-report-2024-year-of-stablecoins), [BitPay 2025](https://www.bitpay.com/decrypted/2025), [BitPay at 15 years](https://www.bitpay.com/resources/15-years-of-building). All figures are the companies' own.

- **What people buy.** BitPay's top industries in 2024 were sports, precious metals, VPN and hosting, computer networking, luxury goods and cars ([BitPay](https://www.bitpay.com/blog/2024-year-in-review)). CoinGate names digital services, software and subscriptions.
- **Lightning is small here.** CoinGate's Lightning share of bitcoin payments fell from 15.4% in 2024 to 11.3% in 2025. That's roughly 35,000 Lightning payments in a year *[our arithmetic]*.
- **BTCPay Server** can't count its users' payments; its 2025 report gives anecdotes only ([BTCPay Server](https://blog.btcpayserver.org/2025-report/)).

**What it shows:** people who pay through processors already hold crypto and spend what they hold; bitcoin is about a fifth of it. Merchants mostly take local money, as elsewhere in this library.

## Where the recipient asks for bitcoin

Method principle 5 says to look beyond the respectable. These are the places where sellers ask for bitcoin because other payments are closed to them, or because they want distance from banks.

- **Gambling.** Estimates of crypto casinos' gross gaming revenue for 2024 run from about $10–11 billion ([Earnings+More, citing Tanzanite](https://earningsandmore.substack.com/p/calling-bull)) to $81.4 billion ([Daily Hodl, citing Yield Sec](https://dailyhodl.com/2025/04/22/crypto-gambling-generates-81400000000-in-gross-revenue-at-casinos-last-year-despite-regulatory-bans-report/)). The largest operator, Stake, claims $4.7 billion, and says over half its transactions are in fiat ([IMGL Magazine](https://www.imgl.org/publications/imgl-magazine-volume-3-no-1/the-rise-and-rise-of-crypto-casino-and-what-can-be-done-to-stop-it-if-anything/), 2025). Bitcoin is losing ground: at one platform vendor, "Bitcoin's share dropped by over 17 percentage points" of crypto bets in 2024, while Tether and Litecoin gained ([SOFTSWISS](https://www.softswiss.com/knowledge-hub/state-of-crypto-2024/)). No source gives bitcoin's absolute share.
- **Darknet markets.** Inflows were just over $2.5 billion in 2025 ([Chainalysis](https://www.chainalysis.com/blog/crypto-drug-sales-darknet-markets-2026/)) and just over $2 billion in bitcoin in 2024. But "Many operators have since moved to accepting only Monero," which the figures leave out ([Chainalysis](https://www.chainalysis.com/blog/darknet-markets-2025/)). In 2025, 48% of newly launched markets took only Monero ([TRM Labs](https://trmlabs.com/resources/blog/monero-in-2025-persistent-use-and-emerging-network-layer-insights)).
- **Ransomware.** Payments were about $820 million in 2025, down from $892 million ([Chainalysis](https://www.chainalysis.com/blog/crypto-ransomware-2026/)); 28% of victims paid ([The Register](https://www.theregister.com/2026/02/27/ransomware_chainalysis/)). "The overwhelming majority of ransom payments are still made in bitcoin" ([TRM Labs](https://trmlabs.com/resources/blog/monero-in-2025-persistent-use-and-emerging-network-layer-insights)). This is extortion, not demand, but it is the clearest case of a recipient dictating the currency.
- **Privacy and internet services.** Mullvad has accepted bitcoin since 2010 and gives 10% off for crypto "due to lower fees and less administration" ([Mullvad](https://mullvad.net/en/pricing), [Mullvad, 2010](https://mullvad.net/en/blog/bitcoin-payments)). IVPN runs its own BTCPay server ([IVPN](https://www.ivpn.net/knowledgebase/general/what-payment-methods-do-you-accept/)). Namecheap took over $73 million in bitcoin across 1.1 million transactions from May 2020 to October 2024, from over 500,000 users ([BTCPay Server](https://blog.btcpayserver.org/case-study-namecheap/), a vendor case study). None publishes what share of customers pay this way.

**What it shows:** the sellers who ask for bitcoin are those shut out of cards or serving buyers who want privacy. Where they have a choice of coin, they are moving to stablecoins for stability and Monero for privacy. Bitcoin keeps the cases where it was first and where buyers already hold it.

## Uses bitcoin had, and lost

| What | When | What happened |
| --- | --- | --- |
| ChangeTip (tipping on social media) | 2016 | Closed; the team was hired by Airbnb ([Bitcoin.com News](https://news.bitcoin.com/bitcoin-tipping-changetip-closes-doors)) |
| Dell | 2014–2017 | Dropped bitcoin, citing "low demand" ([U.Today](https://u.today/dell-ceo-michael-dell-snubs-bitcoin)) |
| Steam | 2017 | Dropped it: "These fees result in unreasonably high costs for purchasing games when paying with Bitcoin" ([The Next Web](https://thenextweb.com/news/bitcoin-valve-steam-payments)) |
| Microsoft | January 2018 | Paused bitcoin payments; employees cited instability ([Bleeping Computer](https://www.bleepingcomputer.com/news/cryptocurrency/microsoft-halts-bitcoin-transactions-because-its-an-unstable-currency-/)) |
| Stripe | 2018 | Ended support: bitcoin had "become better-suited to being an asset than being a means of exchange"; fees of "tens of U.S. dollars" were common and merchants' interest had fallen ([Stripe](https://stripe.com/blog/ending-bitcoin-support)). Stripe later added stablecoins. |
| Expedia | 2018 | Stopped without giving a reason ([CoinGeek](https://coingeek.com/btc-loses-another-major-company-expedia-removes-btc-payments-website/)) |
| Merchant processors overall | 2018 | Bitcoin volume at 17 merchant services fell from $344.2 million in January to $95.6 million in September ([Digital Transactions, citing Chainalysis](https://www.digitaltransactions.net/bitcoins-renewed-volatility-casts-a-spotlight-on-its-shrinking-merchant-volume/)) |
| BitPay | 2020–2021 | Bitcoin fell from 92% to about 65% of transactions ([FXStreet](https://www.fxstreet.com/cryptocurrencies/news/bitcoin-payments-decline-as-other-cryptocurrencies-grow-202201171049)) |
| Purse (discounted Amazon orders paid in bitcoin) | 2020, 2023 | Announced closure in 2020 ([The Block](https://www.theblock.co/post/62220/bitcoins-killer-app-purse-is-shutting-down-open-to-acquisition-opportunities)), reversed it, and wound down in 2023 *[to verify: the 2023 announcement couldn't be opened]* |
| Tippin.me (Lightning tips) | 2023 | Its node went offline with no announcement; users couldn't withdraw ([No Bullshit Bitcoin](https://nobsbitcoin.com/tippin-me-potential-rug-pull)) |
| CoinGate | 2023–2025 | Bitcoin fell from 35.6% to about 22% of payments ([CoinGate](https://coingate.com/blog/post/crypto-payments-report-2024-year-of-stablecoins)) |

**What it shows:** bitcoin was once the only coin at checkout. Merchants left when on-chain fees and price swings peaked in late 2017, and they gave low demand as often as cost. Lightning fixed the fees; the merchants didn't come back, and stablecoins took the growth. Tipping products closed twice, a decade apart.

## Remittances: the one measured series

El Salvador's central bank counts remittances received through crypto wallets. The category covers all crypto, not only bitcoin.

| Period | Through crypto wallets | Share of all remittances |
| --- | --- | --- |
| September 2021 – July 2023 | $236.7 million | 1.6% |
| January–August 2024 | $57.4 million | 1.1% |
| 2025 | $57.7 million | about 0.5% in January–April |
| First half of 2026 | $35.4 million | 0.7% |

Sources: [Diario El Mundo, 2023](https://diario.elmundo.sv/economia/1-de-cada-100-en-remesas-se-ha-enviado-en-bitcoin-desde-septiembre-de-2021), [Bitcoin.com News](https://news.bitcoin.com/central-reserve-bank-only-1-1-of-remittances-involve-cryptocurrency-in-el-salvador), [Diario El Mundo, 2025](https://diario.elmundo.sv/economia/las-remesas-en-billeteras-de-criptomonedas-caen-un-445-en-el-salvador), [Blockhead](https://www.blockhead.co/2026/07/29/the-bitcoin-experiments-five-year-report-card-35-4-million/). All relay central bank data.

**What it shows:** in the country that tried hardest, crypto's share of remittances fell from under 2% to under 1%. No bitcoin-only or Lightning-only remittance figure exists anywhere.

## The people who already hold bitcoin

Holders are the nearest source of spending, since they don't have to buy first.

- **A growing share can't be spent.** US spot ETFs hold about 1.26 million BTC, public companies 1.23 million and governments 0.52 million ([Bitbo](https://bitbo.io/treasuries/), November 10, 2026). Together that's about 3 million coins, around 14% of the 21 million limit *[our arithmetic]*. In 2025, "Individuals sold 696,000 BTC… while businesses, funds & ETFs, and governments bought nearly 1 million" ([River](https://river.com/content/bitcoin-adoption-2026)).
- **Most coins don't move.** About 64% of bitcoin last moved more than a year ago ([Glassnode](https://studio.glassnode.com/charts/supply.HodlWaves?a=BTC), November 10, 2026) *[our sum of six age bands; includes lost coins and coins in funds]*.
- **Owners invest; few pay.** In the US, 9% of adults held crypto as an investment in 2025 and 2% paid with it ([Federal Reserve](https://www.federalreserve.gov/publications/2026-economic-well-being-of-us-households-in-2025-banking.htm)). The share paying fell from nearly 3% in 2021–2022 ([Kansas City Fed](https://www.kansascityfed.org/research/payments-system-research-briefings/us-consumers-use-of-cryptocurrency-for-payments/)). In Germany, of the 7% who had bought or paid with crypto, "9 out of 10 said they use their tokens primarily to invest. 8% said they also use them to pay" ([Bundesbank](https://www.bundesbank.de/resource/blob/997852/1b30fa6978e2f05229d91beceeaf78cc/472B63F073F071307366337C94F8C870/zahlungsverhalten-in-deutschland-2025-data.pdf), 2025).
- **Those who spend, spend dollars.** Tracked crypto card spending reached $759 million in July 2026, up from $306 million a year earlier; USDC funded about 58% and USDT about 26% ([Crypto Briefing, citing Paymentscan](https://cryptobriefing.com/crypto-card-sector-250-projects-monthly-spending/)). No source gives bitcoin's share.
- **Or they borrow instead of selling.** Crypto-backed lending stood at $56.16 billion in June 2026 ([Galaxy](https://www.galaxy.com/insights/research/crypto-leverage-report-q2-2026-defi-lending-decline-futures-open-interest), all collateral types). Coinbase's bitcoin-backed loans passed $1 billion in originations in September 2025 ([The Block](https://www.theblock.co/post/373032)). How much of that money is spent on everyday things isn't known.
- **Rewards add bitcoin to card spending, in small amounts.** Fold reported 625,000 accounts and $235 million in quarterly transaction volume in late 2025 ([Fold](https://www.sec.gov/Archives/edgar/data/1889123/000119312525274190/fld-ex99.htm)); Lolli had paid out over $20 million in bitcoin to 600,000 users by mid-2025 ([The Block](https://www.theblock.co/post/360747/thesis-lolli-acquisition-bitcoin-rewards)). The spending itself is in dollars.

### Tax

- **In the US, every purchase is a taxable sale.** A $300 exemption (S.2207) was still in committee in August 2026 ([CoinTracking](https://cointracking.info/blog/crypto-de-minimis-tax-exemption)). The bill that advanced in the House in September 2026 exempts only network fees of $10 or less, while giving dollar stablecoins no-gain treatment ([EY](https://taxnews.ey.com/news/2026-1972-ways-and-means-approves-digital-assets-tax-bill), [Forvis Mazars](https://www.forvismazars.us/forsights/2026/09/ways-means-approves-digital-asset-tax-certainty-act)).
- **Germany and Portugal exempt bitcoin held for a year** ([CoinTracking](https://cointracking.info/blog/germany-crypto-holding-period-reform-2026), [LVP Advogados](https://www.lvpadvogados.com/crypto-assets-in-portugal-current-tax-framework-and-key-developments)). Germany's finance minister has signaled a change from 2027 ([Cointelegraph](https://cointelegraph.com/news/germany-signals-2027-crypto-tax-overhaul-one-year-holding-perk-under-threat)).
- **No study measures the effect.** Germans can spend long-held bitcoin tax-free, and about nine in ten German crypto owners still use it primarily to invest. That suggests tax isn't the main barrier *[assumption: no source tests this]*.

## What people say, and what they do

**Say:** in a survey of over 5,700 bitcoin holders by a mining company, 55% rarely or never spend crypto, and blame merchant acceptance (49%), fees (45%) and volatility (43%) ([CryptoPotato on GoMining](https://cryptopotato.com/gomining-survey-shows-55-of-bitcoiners-never-use-it-for-real-world-payments/)). *A company survey, not a representative sample.*

**Do:** about 1 million Square sellers are enabled to accept bitcoin and no usage is published; Lightning removed the fees that drove merchants away in 2017, and they didn't return. Among Americans who do pay with crypto, the top reason is that the recipient preferred it: 26% in 2025 ([Federal Reserve](https://www.federalreserve.gov/publications/2026-economic-well-being-of-us-households-in-2025-banking.htm)) and over 35% in 2024 ([Kansas City Fed](https://www.kansascityfed.org/research/payments-system-research-briefings/us-consumers-use-of-cryptocurrency-for-payments/)).

**Say versus do:** holders say acceptance and fees stop them. Where both were fixed, spending didn't follow. People pay in bitcoin when the other side asks for it.

## What it means for the research areas

| Area | What changes |
| --- | --- |
| 11 Community-driven economies | Organizers cut off from cards (adult creators, some fan projects) resemble the sellers who ask for bitcoin today; most group orders don't |
| 12 Earning in bitcoin | Rewards and converted pay add bitcoin to savings; there's no evidence they add spending |
| 13 Agentic payments | The same shift as at processors and casinos: bitcoin first, stablecoins for growth |
| 14 Dollars and bitcoin | Holders who spend already use dollars (cards, loans). The question is whether bitcoin wallets serve that or leave it to others |
| 15 Money that can't be frozen | The largest "recipient asks" flows are gray or illicit, and they are moving to Monero where privacy matters |
| 17 Brand and culture as demand | Lightning volume as a headline number is reach, not use |
| 18 Last-mile infrastructure | Exchange deposits and withdrawals are Lightning's largest real use: moving in and out is the product |

## What isn't published

1. The share of Lightning volume that pays for goods or services, as opposed to exchange transfers.
2. The value of bitcoin payments at any processor (CoinGate gives counts, BitPay rankings).
3. Bitcoin payments received by Square sellers.
4. Bitcoin's share of deposits at any gambling operator.
5. Bitcoin against Monero on darknet markets, by volume.
6. The share of customers paying in bitcoin at any VPN, registrar or host.
7. Bitcoin's share of crypto card spending.
8. How much money borrowed against bitcoin is spent.
9. Why holders don't spend, from a survey that offers tax and "I expect the price to rise" as answers.

## Open questions

1. What do people buy with the bitcoin they move off exchanges over Lightning, if anything?
2. Why did merchants not return once Lightning removed fees: low demand, volatility, tax, or habit?
3. Are there holders who spend regularly? Who are they, what do they buy, and do they buy the bitcoin back?
4. Does a one-year tax exemption change spending in Germany or Portugal?
5. Where sellers have moved from bitcoin to stablecoins or Monero, what would they have needed to stay?

## Sources

**Lightning:** [River: Bitcoin adoption 2026](https://river.com/content/bitcoin-adoption-2026) · [River's 2026 report](https://river.com/learn/files/river-bitcoin-adoption-report-2026.pdf) · [River's 2023 Lightning report](https://river.com/learn/files/river-lightning-report-2023.pdf) · [Lightspark on Coinbase](https://www.lightspark.com/blog/news/coinbase-lightning-network-lightspark) · [CoinDesk on Block](https://www.coindesk.com/tech/2025/05/29/square-flies-the-flag-for-the-lightning-network-with-97-yield-on-bitcoin-holdings)

**Processors:** [CoinGate 2025 report](https://coingate.com/blog/post/crypto-payments-data-report-2025) · [CoinGate 2024 report](https://coingate.com/blog/post/crypto-payments-report-2024-year-of-stablecoins) · [BitPay 2025](https://www.bitpay.com/decrypted/2025) · [BitPay at 15 years](https://www.bitpay.com/resources/15-years-of-building) · [BitPay 2024 review](https://www.bitpay.com/blog/2024-year-in-review) · [BTCPay Server 2025 report](https://blog.btcpayserver.org/2025-report/)

**Where the recipient asks:** [Earnings+More on casino estimates](https://earningsandmore.substack.com/p/calling-bull) · [Daily Hodl on Yield Sec](https://dailyhodl.com/2025/04/22/crypto-gambling-generates-81400000000-in-gross-revenue-at-casinos-last-year-despite-regulatory-bans-report/) · [IMGL Magazine on crypto casinos](https://www.imgl.org/publications/imgl-magazine-volume-3-no-1/the-rise-and-rise-of-crypto-casino-and-what-can-be-done-to-stop-it-if-anything/) · [SOFTSWISS: State of crypto 2024](https://www.softswiss.com/knowledge-hub/state-of-crypto-2024/) · [Chainalysis on darknet markets, 2026](https://www.chainalysis.com/blog/crypto-drug-sales-darknet-markets-2026/) · [Chainalysis on darknet markets, 2025](https://www.chainalysis.com/blog/darknet-markets-2025/) · [TRM Labs on Monero](https://trmlabs.com/resources/blog/monero-in-2025-persistent-use-and-emerging-network-layer-insights) · [Chainalysis on ransomware](https://www.chainalysis.com/blog/crypto-ransomware-2026/) · [The Register on ransomware](https://www.theregister.com/2026/02/27/ransomware_chainalysis/) · [Mullvad pricing](https://mullvad.net/en/pricing) · [Mullvad, 2010](https://mullvad.net/en/blog/bitcoin-payments) · [IVPN payment methods](https://www.ivpn.net/knowledgebase/general/what-payment-methods-do-you-accept/) · [BTCPay Server on Namecheap](https://blog.btcpayserver.org/case-study-namecheap/)

**Lost uses:** [Stripe: ending bitcoin support](https://stripe.com/blog/ending-bitcoin-support) · [The Next Web on Steam](https://thenextweb.com/news/bitcoin-valve-steam-payments) · [U.Today on Dell](https://u.today/dell-ceo-michael-dell-snubs-bitcoin) · [Bleeping Computer on Microsoft](https://www.bleepingcomputer.com/news/cryptocurrency/microsoft-halts-bitcoin-transactions-because-its-an-unstable-currency-/) · [CoinGeek on Expedia](https://coingeek.com/btc-loses-another-major-company-expedia-removes-btc-payments-website/) · [Digital Transactions on merchant volume](https://www.digitaltransactions.net/bitcoins-renewed-volatility-casts-a-spotlight-on-its-shrinking-merchant-volume/) · [FXStreet on BitPay's bitcoin share](https://www.fxstreet.com/cryptocurrencies/news/bitcoin-payments-decline-as-other-cryptocurrencies-grow-202201171049) · [Bitcoin.com News on ChangeTip](https://news.bitcoin.com/bitcoin-tipping-changetip-closes-doors) · [No Bullshit Bitcoin on Tippin.me](https://nobsbitcoin.com/tippin-me-potential-rug-pull) · [The Block on Purse](https://www.theblock.co/post/62220/bitcoins-killer-app-purse-is-shutting-down-open-to-acquisition-opportunities)

**Remittances:** [Diario El Mundo, 2023](https://diario.elmundo.sv/economia/1-de-cada-100-en-remesas-se-ha-enviado-en-bitcoin-desde-septiembre-de-2021) · [Bitcoin.com News on 2024](https://news.bitcoin.com/central-reserve-bank-only-1-1-of-remittances-involve-cryptocurrency-in-el-salvador) · [Diario El Mundo, 2025](https://diario.elmundo.sv/economia/las-remesas-en-billeteras-de-criptomonedas-caen-un-445-en-el-salvador) · [Blockhead on 2026](https://www.blockhead.co/2026/07/29/the-bitcoin-experiments-five-year-report-card-35-4-million/)

**Holders:** [Bitbo treasuries](https://bitbo.io/treasuries/) · [Glassnode HODL waves](https://studio.glassnode.com/charts/supply.HodlWaves?a=BTC) · [Federal Reserve: Economic Well-Being of US Households in 2025](https://www.federalreserve.gov/publications/2026-economic-well-being-of-us-households-in-2025-banking.htm) · [Kansas City Fed on crypto payments](https://www.kansascityfed.org/research/payments-system-research-briefings/us-consumers-use-of-cryptocurrency-for-payments/) · [Bundesbank: Payment behaviour in Germany 2025](https://www.bundesbank.de/resource/blob/997852/1b30fa6978e2f05229d91beceeaf78cc/472B63F073F071307366337C94F8C870/zahlungsverhalten-in-deutschland-2025-data.pdf) · [Crypto Briefing on crypto cards](https://cryptobriefing.com/crypto-card-sector-250-projects-monthly-spending/) · [Galaxy on crypto lending](https://www.galaxy.com/insights/research/crypto-leverage-report-q2-2026-defi-lending-decline-futures-open-interest) · [The Block on Coinbase's loans](https://www.theblock.co/post/373032) · [Fold Q3 2025 results](https://www.sec.gov/Archives/edgar/data/1889123/000119312525274190/fld-ex99.htm) · [The Block on Lolli](https://www.theblock.co/post/360747/thesis-lolli-acquisition-bitcoin-rewards) · [CryptoPotato on the GoMining survey](https://cryptopotato.com/gomining-survey-shows-55-of-bitcoiners-never-use-it-for-real-world-payments/)

**Tax:** [CoinTracking on the de minimis exemption](https://cointracking.info/blog/crypto-de-minimis-tax-exemption) · [EY on the Digital Asset Tax Certainty Act](https://taxnews.ey.com/news/2026-1972-ways-and-means-approves-digital-assets-tax-bill) · [Forvis Mazars on the same bill](https://www.forvismazars.us/forsights/2026/09/ways-means-approves-digital-asset-tax-certainty-act) · [CoinTracking on Germany](https://cointracking.info/blog/germany-crypto-holding-period-reform-2026) · [Cointelegraph on Germany's 2027 plans](https://cointelegraph.com/news/germany-signals-2027-crypto-tax-overhaul-one-year-holding-perk-under-threat) · [LVP Advogados on Portugal](https://www.lvpadvogados.com/crypto-assets-in-portugal-current-tax-framework-and-key-developments)

*Research for this draft was done with AI agents, each claim taken from a source an agent opened. Nothing here has been rechecked by hand yet, and no claims list exists for this page.*
