# Money that can't be frozen

*Deep dive, first draft. Builds on the November 8 quick scan. Desk research only. Last updated November 11, 2026.*

## Thesis

Bitcoin's clearest advantage over stablecoins and banks is that nobody can freeze, seize or block it. Most people don't weigh this until it happens to them. The evidence below suggests three things about when it matters:

- **Demand is episodic.** People turn to bitcoin at the moment they're cut off: to receive donations after a blockade, or to carry savings across a border. Few keep using it for payments once the crisis passes.
- **Self-custody, not the asset, is what survives.** In the 2022 Canadian convoy freezes, bitcoin sent wallet to wallet reached its recipients; funds held by exchanges and banks were frozen. Bitcoin held by a custodian can be frozen like anything else.
- **The chokepoints have moved to the edges.** Miners rarely block transactions. Custodial wallets leaving countries, app stores, service operators and legal pressure on wallet developers are where access actually gets cut.

Meanwhile, the everyday workarounds in crisis economies run on stablecoins that *can* be frozen, because they hold their value and everyone already uses them.

**The hypothesis:** censorship resistance creates demand that is small, urgent and unpredictable. Products that serve it have to be ready *before* the crisis: already installed, not dependent on one operator or one app store, private by default, and simple enough to set up under stress.

*Status: a working hypothesis from desk research. What people actually do in the days after they're cut off is the main gap; public cases describe the fundraising, rarely what came next.*

## What we mean

**Who can freeze money:**

| Who | How | Example |
| --- | --- | --- |
| Stablecoin issuers | Blacklisting addresses | Tether, Circle ([Dollars and bitcoin](14-dollars-and-bitcoin.md)) |
| Banks and payment processors | Closing accounts, refusing transactions | Debanking; card networks and adult content |
| Governments | Emergency powers, court orders, sanctions, exchange bans | Canada 2022, Nigeria 2024 |
| Custodial services | Freezing balances, leaving a country | Exchanges, custodial Lightning wallets |
| Infrastructure operators | Refusing to process | Ark operators, ecash mints, Lightning service providers |
| App stores | Removing apps by country | China, Russia |

**Three jobs** that people need censorship-resistant money for:

1. **Receiving** when cut off: donations, sales.
2. **Saving and carrying** value out of reach: across a border, out of a failing bank.
3. **Paying** for everyday things without permission.

The evidence is strongest for the first two.

## What people say, and what they do

**Say:** bitcoiners call censorship resistance bitcoin's killer feature. Activists praise it: a Nigerian protest group said bank restrictions forced it to "only accept donations in bitcoin" ([Bitcoin Magazine](https://bitcoinmagazine.com/culture/nigerian-protest-group-finds-sovereign-lifeline-in-bitcoin), October 2020).

**Do:**

- **Bitcoin is a minority channel, converted quickly.** Russia's opposition foundation FBK received over 653 BTC at its public address between 2016 and 2021 but never held more than about $110,000 at once ([Protos](https://protos.com/alexei-navalny-bitcoin-donations-putin/), January 2021). A senior aide said crypto made up 10–15% of donations, was converted to rubles quickly, and served mainly as a "deterrent" against blocking the other channels ([Moscow Times](https://www.themoscowtimes.com/2026/09/10/russian-opposition-finds-refuge-in-bitcoin)). *[to verify: the page's date doesn't match its URL]*
- **Bitcoin's share fell in Ukraine's crypto donations.** In the first two weeks of the 2022 invasion, $63.8 million arrived in over 120,000 donations: ether 33.7%, bitcoin 31.2%, stablecoins 17% ([Elliptic](https://www.elliptic.co/insights/live-updates-ukraine-government-turns-to-crypto-to-crowdfund-millions-of-dollars), March 2022). By May 2023 the total passed $212 million, with "comparatively lower reliance on Bitcoin" ([Elliptic](https://elliptic.co/blog/analysis/crypto-donations-to-ukraine-and-russia-breaking-down-the-numbers)).
- **Crisis workarounds run on stablecoins.** Peer-to-peer crypto trading worldwide "is now 96% stablecoins," by Chainalysis's 2026 measure, which counts domestic bitcoin transfers only below $10,000 ([Chainalysis](https://www.chainalysis.com/blog/2026-global-crypto-adoption-index/), September 2026).
- **Bitcoin shows up for savings and flight.** In collapsing currencies, people split the job: stablecoins to spend, bitcoin to save. Iran saw about $8 billion in crypto activity through Iranian addresses in 2025; people use stablecoins such as Tether for everyday transactions and hold bitcoin as long-term savings, much as Lebanese did when the pound lost 90% of its value in 2019–2021 ([Pulse on CoinDesk](https://www.pulse.bot/crypto/news/irans-rial-collapse-mirrors-lebanons-crisis-driving-citizens-to-bitcoin-dab77748-d289-40ae-b5a0-35bbf0d403d1), February 2026).

**Say versus do:** censorship resistance pulls people toward bitcoin mainly when someone actually freezes or blocks them. Even then it's one channel among several, and money usually leaves bitcoin quickly.

## Why existing payments fail them

- **Card networks decide what legal businesses can sell.** In July 2025, Steam added a rule against content that may break the standards of payment processors, card networks and banks, and delisted many adult games ([Notebookcheck](https://www.notebookcheck.net/Steam-tightens-adult-content-rules-after-pressure-from-payment-giants.1059462.0.html)). itch.io followed, and DLsite had already lost Visa and Mastercard in 2024 ([Community-driven economies](11-community-driven-economies.md)).
- **Banks close accounts, often without saying why.** In a survey of about 400 sex workers, over 40% had lost a financial account in the past year ([Boston Globe](https://www.bostonglobe.com/2023/06/01/business/digital-payment-platforms-shutting-out-sex-workers), 2023).
- **Debanking is political, in every direction.** An August 2025 US executive order directs regulators to stop "politicized or unlawful debanking," citing firearms dealers, payday lenders and tobacco companies cut off under the Obama-era Operation Choke Point ([Cooley](https://www.cooley.com/news/insight/2025/2025-08-14-executive-order-guarantees-efforts-against-debanking-will-continue)). The OCC's resulting review found the nine largest banks had restricted sectors including firearms, coal, Arctic oil and gas, detention facilities, tobacco and digital assets, but could not quantify how many customers were affected ([Sidley](https://www.sidley.com/en/insights/newsupdates/2026/10/office-of-the-comptroller-of-the-currency-issues-final-report-on-debanking), October 2026). The Cato Institute counters that of over 8,300 complaints about closed accounts since 2012, only 35 mention politics or religion, and that anti-money-laundering rules drive most closures ([American Banker](https://www.americanbanker.com/news/cato-report-says-administration-misdiagnosed-debanking), January 2026). Which businesses get cut off shifts with politics; that it happens doesn't.
- **Governments freeze accounts in emergencies.** Canada's use of the Emergencies Act against the 2022 convoy protests was ruled unreasonable by the Federal Court in 2024 and by the Federal Court of Appeal in January 2026, which found the order requiring banks to disclose protesters' property breached the Charter's protection against unreasonable search ([Federal Court of Appeal](https://www.fca-caf.ca/en/pages/decisions/plain-language-decision-summaries/2026-fca-6)). The Supreme Court agreed to hear the government's appeal ([CP24](https://www.cp24.com/news/canada/2026/10/22/supreme-court-to-hear-federal-appeal-over-use-of-emergencies-act/), October 2026).
- **Stablecoins can be frozen,** and are: over $514 million in 30 days this spring, and US law requires issuers to be able to freeze ([Dollars and bitcoin](14-dollars-and-bitcoin.md)). Spiral sees possible catalysts in a US crackdown on stablecoin wallets that don't check ID, and in countries restricting dollar stablecoins, as Brazil did for cross-border settlement ([Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)).

## Case studies

### Donations under blockade

- **WikiLeaks, 2010.** A payment blockade by card networks and PayPal cost WikiLeaks 95% of its revenue, by its own account ([Christian Science Monitor](https://www.csmonitor.com/World/Latest-News-Wires/2011/1024/Wikilieaks-says-financial-blockade-could-put-it-out-of-business), 2011). Its bitcoin address, opened in June 2011, received over 25,000 donations and passed 4,000 BTC by November 2016, worth about $177,000 when received ([Bitcoin Magazine](https://bitcoinmagazine.com/culture/wikileaks-public-donation-address-receives-th-bitcoin-1480629241)).
- **Nigeria's Feminist Coalition, 2020.** During the #EndSARS protests, Flutterwave cut off the group's donation accounts. It first used a service converting bitcoin into naira, dropped it over the risk of bank freezes, then set up a self-hosted BTCPay Server and raised about 3.14 BTC (about $36,000 at the time) ([CoinDesk](https://www.coindesk.com/nigerian-activists-bitcoin-endsars-police-brutality/)).
- **Canada, 2022.** After GoFundMe froze over $9 million, convoy supporters raised about 22 BTC on Tallycoin. Organizers sent 14.6 BTC to 90 truckers wallet to wallet before police ordered regulated firms to stop dealing with 34 wallets and a court froze at least 146 more ([Fortune](https://fortune.com/2022/02/18/freedom-convoy-protests-canada-lawsuit-freeze-crypto-wallets-ottawa)). Kraken's CEO, on funds held at exchanges: "We cannot protect you."
- **Ukraine, 2022.** The largest crypto fundraiser on record, but led by ether and stablecoins (above).

**What it shows:** bitcoin works as the channel of last resort when others close. What reaches people is what's self-custodied. Public records rarely say whether the groups kept using bitcoin afterwards.

### Creators and businesses cut off

- **Adult games, 2025.** Reporting on the Steam and itch.io delistings found no move to crypto payments; a developer noted that many crypto payment tools are themselves centralized, and the campaign group behind the pressure said it had discussed targeting crypto processors next ([Decrypt](https://decrypt.co/332395/pressure-group-forced-steam-remove-adult-games-coming-after-crypto-next), July 2025).
- **Sex workers.** Crypto "stumbled" after FTX's collapse, and a crypto payment platform for sex work was targeted for shutdown when its own provider dropped adult businesses ([Boston Globe](https://www.bostonglobe.com/2023/06/01/business/digital-payment-platforms-shutting-out-sex-workers)). The basic barrier: clients don't use crypto ([KQED](https://www.kqed.org/news/11899955/when-banks-turned-their-backs-on-them-some-adult-entertainment-workers-turned-to-cryptocurrency)).
- **Debanked businesses.** No public evidence shows US firearms, tobacco or crypto firms turning to bitcoin payments when debanked; they needed banks for payroll and suppliers.

**What it shows:** for sellers, censorship resistance only helps if buyers can pay. That's a demand problem on the buyer's side, not a technology problem.

### Crisis economies: saving and leaving

- **Stablecoins for daily life.** In Venezuela, USDT is used "for everything from groceries and apartment fees to salaries" ([Sumsub](https://sumsub.com/media/news/stablecoins-used-in-venezuela-amid-inflation-fears/), September 2025). Russian businesses cutting around sanctions have long chosen USDT ([Elliptic](https://www.elliptic.co/insights/the-fall-of-a7a5-how-sanctions-strangled-the-ruble-stablecoin/), July 2026). Myanmar's opposition government runs payments on a tokenized kyat and a USDT copy ([Elliptic](https://www.elliptic.co/insights/the-digital-kyat-tracing-the-cbdc-financing-over-11-5-million-in-civil-war-donations-to-myanmars-opposition/), April 2025).
- **Bitcoin for buying and saving.** On Nigerian exchanges, bitcoin is 89% of crypto purchases ([Chainalysis](https://www.chainalysis.com/blog/subsaharan-africa-crypto-adoption-2025/), September 2025), while Nigeria ranks first in the world for peer-to-peer trading, which is mostly stablecoins ([Chainalysis](https://www.chainalysis.com/blog/2026-global-crypto-adoption-index/)).
- **Bitcoin for leaving.** A young Ukrainian crossed into Poland in 2022 with about $2,000 in bitcoin: "I could just write my seed phrase on a piece of paper" ([CNBC](https://www.cnbc.com/2022/03/23/ukrainian-flees-to-poland-with-2000-in-bitcoin-on-usb-drive.html)). Lebanese traders reported millions of dollars a month in bitcoin trades after banks imposed controls in 2019, yet it "never really took off," held back by card limits, slow internet and power cuts ([Al Jazeera](https://www.aljazeera.com/economy/2020/2/25/distrust-in-lebanese-banks-spurs-bitcoin-boom), February 2020). In Sudan's war, a family fleeing to Ethiopia received cash from a trader paid in bitcoin, carrying no money or phones on the road ([No Bullshit Bitcoin, reposting Forbes](https://nobsbitcoin.com/how-bitcoin-helps-civilians-escape-the-war-in-sudan), 2023). During Iran's protests, bitcoin withdrawals from Iranian exchanges to personal wallets rose sharply ([The Block, citing Chainalysis](https://www.theblock.co/post/385941/iran-crypto-ecosystem-irgc-footprint-bitcoin-withdrawals-surge-during-protests-chainalysis), January 2026).
- **Crackdowns move activity, not end it.** After Nigeria detained two Binance executives in 2024, trading moved to WhatsApp, Telegram and other exchanges ([Techpoint](https://techpoint.africa/2024/03/04/more-p2p-takes-place-on-whatsapp/)). After the Taliban took over Afghanistan, crypto received fell from about $68 million a month to under $80,000 ([Cointelegraph](https://cointelegraph.com/news/taliban-had-a-massive-chilling-effect-on-afghan-crypto-market-report), 2022).

**What it shows:** people pick the asset for the job. Freezable stablecoins win daily use because they're stable and liquid; bitcoin wins when the goal is to hold or carry value out of reach. The same pattern appears in [Dollars and bitcoin](14-dollars-and-bitcoin.md).

## Where access actually gets cut

| Layer | Who can block | Evidence | Fallback |
| --- | --- | --- | --- |
| On-chain | Individual mining pools | F2Pool left out sanctioned transactions in 2023; other pools mined them within minutes to hours ([b10c](https://b10c.me/observations/08-missing-sanctioned-transactions/)) | Other miners |
| Lightning, custodial | The wallet company | Wallet of Satoshi left the US in 2023 ([The Block](https://www.theblock.co/post/264585/wallet-of-satoshi-bitcoin-lightning)); its custodial wallet stopped working in several EU countries in early 2026 ([The Rage](https://www.therage.co/wallet-of-satoshi-eu-mica/)) | Move to self-custody, if prepared |
| Lightning, self-custodial | Service providers; the developer's legal exposure | Phoenix left the US in 2024, citing doubt over whether self-custodial wallet providers or Lightning service providers count as money transmitters ([Cointelegraph](https://cointelegraph.com/news/phoenix-wallet-acinq-zksnacks-wasabi-wallet-united-states-crackdown)). It announced its return in April 2025, the day after the Justice Department's memo (below) ([bitcoin.fr](https://bitcoin.fr/phoenix-wallet-de-retour-aux-usa/)) | Other providers or own node |
| Lightning, network | Internet providers | A network operator "can identify and censor all payments routed via their network" ([AFT 2024](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.AFT.2024.12)) | Tor, other routes |
| Ark (Arkade) | The operator | The operator can't spend users' funds but can refuse them; "There is one operator" ([Arkade docs](https://docs.arkadeos.com/learn/faq/what-if-the-operator-disappears-or-acts-maliciously)) | Unilateral exit on-chain, paying fees, before the batch expires |
| Spark | Its operators | Funds are "recoverable on L1 via a unilateral exit" ([Spark docs](https://docs.spark.money/learn/tldr.md)) | Unilateral exit |
| Fedimint | A majority of guardians | Could collude to steal; can't see balances ([Fedimint](https://fedimint.org/users/privacy-and-trust)) | None if the majority acts |
| Cashu | The mint | Holds the funds and has "the power to censor certain payments" ([Cashu FAQ](https://docs.cashu.space/faq)) | None |
| App stores | Apple, Google, at a government's request | Apple removed a chat app from China's store in 2015 for adding bitcoin payments ([TechCrunch](https://techcrunch.com/?p=1132099)); Apple removed 1,213 apps at Russia's request in 2025, without naming them ([Meduza](https://meduza.io/en/news/2026/05/25/apple-removed-1-213-apps-at-russia-s-internet-regulator-s-request-in-2025)). Google Play requires licenses for custodial wallets but exempts self-custodial ones ([Decrypt](https://decrypt.co/335134/google-non-custodial-wallets-exempt-new-crypto-app-rules-play-store), 2025) | Sideloading, web apps |
| Wallet developers | Prosecutors | Samourai Wallet's co-founders were sentenced in 2025 for running an unlicensed money transmitting business ([DL News](https://www.dlnews.com/articles/defi/samourai-dev-gets-max-sentence-for-money-transmission-charge/)); zkSNACKs shut Wasabi's coinjoin coordinator in 2024 ([No Bullshit Bitcoin](https://nobsbitcoin.com/zksnacks-to-suspend-its-coinjoin-coordination-service-on-june-1st)). In April 2025 the Justice Department said it would no longer target "offline wallets for the acts of their end users" ([DOJ memo](https://www.justice.gov/dag/media/1395781/dl?inline)) | Open-source code, other jurisdictions |

**What it shows:** the protocol holds up; the edges don't. A wallet's resistance to freezing depends on whether it can exit to the chain, whether it relies on one operator, and whether it can stay installed.

## The rules

| Rule | What it does | Status |
| --- | --- | --- |
| GENIUS Act (US) | Stablecoin issuers must be able to freeze on lawful order | Law since July 2025 ([GENIUS Act](https://www.govinfo.gov/content/pkg/PLAW-119publ27/html/PLAW-119publ27.htm)) |
| FinCEN's unhosted wallet proposal (US) | Would have required banks and money services businesses to report transfers with self-hosted wallets over $10,000 and keep records over $3,000 | Withdrawn October 6, 2026 ([Federal Register](https://public-inspection.federalregister.gov/2026-20430.pdf)) |
| EU Transfer of Funds Regulation | For transfers over €1,000 with a self-hosted address, the exchange must check whether the address belongs to its customer ([Notabene](https://notabene.id/post/key-takeaways-from-the-ebas-consultation-on-travel-rule-guidelines)) *[to verify against the regulation's text]* | Applies since December 30, 2024 ([EBA](https://www.eba.europa.eu/publications-and-media/press-releases/eba-issues-travel-rule-guidance-tackle-money-laundering-and-terrorist-financing-transfers-funds-and)) |
| EU AML Regulation | Bans anonymous accounts at exchanges, but excludes providers of self-hosted wallets ([Didit](https://didit.me/blog/amlr-crypto-casp-requirements/)) *[to verify against the regulation's text]* | From July 2027 |
| FATF (global standard-setter) | Calls peer-to-peer transfers through unhosted wallets "elevated illicit finance risks" and asks exchanges for enhanced checks ([FATF update, via Malta's FIU](https://fiaumalta.org/app/uploads/2026/07/7th-targeted-update-on-implementation-fatf-standards-vas-vasps-2026.pdf.coredownload.pdf)) | Guidance, July 2026 |
| OFAC sanctions (US) | Apply to "miners, wallet providers, and users" alike; encourages geoblocking ([OFAC](https://ofac.treasury.gov/media/913571/download?inline)) | Since 2021 |
| Tornado Cash ruling (US) | Immutable smart contracts aren't property and can't be sanctioned ([Fifth Circuit](https://www.ca5.uscourts.gov/opinions/pub/23/23-50669-CV0.pdf)); Treasury delisted Tornado Cash ([Treasury](https://home.treasury.gov/news/press-releases/sb0057)) | November 2024; March 2025 |
| Account closures (UK) | Payment providers must give 90 days' notice and reasons, with exceptions for crime and money laundering ([SI 2025/688](https://www.legislation.gov.uk/uksi/2025/688/made)) | Since April 28, 2026 |
| Crypto wallet freezing orders (UK) | Courts can freeze crypto suspected to be recoverable property ([Proceeds of Crime Act](https://www.legislation.gov.uk/ukpga/2002/29/section/303Z37)) | Since 2024; whether they reach self-custody is *[to verify]* |

**What it shows:** the US moved toward leaving self-custody alone in 2025–2026; international standards and the EU keep pressure on the points where self-custodied bitcoin meets an exchange.

## Lessons from elsewhere

Do people keep using a tool after the crisis that drove them to it? Messaging apps, VPNs and cash suggest a pattern:

- **Spike, fall, then a higher floor.** After WhatsApp's privacy-policy change in January 2021, Signal's installs grew 5,001% year over year to 50.6 million, fell 86% the next month, and by April were still more than double the year before ([Sensor Tower](https://sensortower.com/blog/whatsapp-signal-telegram-install-growth), 2021). WhatsApp kept its users: people added a tool rather than switching ([Fortune, citing Apptopia](https://fortune.com/2021/02/02/signal-telegram-downloads-surge-facebook-messenger-whatsapp-chat-apps-privacy/)).
- **Use stays high while the block lasts.** VPN demand in Russia peaked at 2,692% above normal in March 2022 and was still 243% above normal at the end of the month; in Myanmar, demand was 464% higher a year after the coup, with Facebook still blocked ([Top10VPN](https://www.top10vpn.com/research/vpn-demand-statistics/)). *Top10VPN reviews VPNs commercially.*
- **Precautionary money stays put.** Euro banknotes issued in the COVID surge were still largely in circulation a year later; issuance in countries next to Ukraine rose 36% and leveled off after about three weeks ([ECB](https://www.ecb.europa.eu/press/economic-bulletin/articles/2025/html/ecb.ebart202506_02~1a773e2ca3.en.html), 2025). In Lebanon, the cash economy grew to 45.7% of GDP in 2022 after confidence in banks collapsed ([The New Arab, citing the World Bank](https://newarab.com/news/lebanons-tanking-economy-cash-based-world-bank)).

**What it suggests:** the right measure of crisis demand is use months later compared with the year before, not the spike. Money held as a precaution is kept, not spent, which fits bitcoin as savings more than bitcoin for payments. Pressure on the tool itself, such as blocking VPNs or removing apps, cuts use too.

## Sizing

| Case | Amount | Source |
| --- | --- | --- |
| WikiLeaks, 2011–2016 | over 4,000 BTC, about $177,000 when received | [Bitcoin Magazine](https://bitcoinmagazine.com/culture/wikileaks-public-donation-address-receives-th-bitcoin-1480629241) |
| FBK, 2016–2021 | over 653 BTC through its address | [Protos](https://protos.com/alexei-navalny-bitcoin-donations-putin/) |
| Feminist Coalition, 2020 | about 3.14 BTC | [CoinDesk](https://www.coindesk.com/nigerian-activists-bitcoin-endsars-police-brutality/) |
| Canada convoy, 2022 | about 22 BTC | [Fortune](https://fortune.com/2022/02/18/freedom-convoy-protests-canada-lawsuit-freeze-crypto-wallets-ottawa) |
| Ukraine, 2022–2023 | over $212 million in crypto, about a third in bitcoin early on | [Elliptic](https://elliptic.co/blog/analysis/crypto-donations-to-ukraine-and-russia-breaking-down-the-numbers) |
| Iran, 2025 | about $8 billion in crypto activity | [Pulse on CoinDesk](https://www.pulse.bot/crypto/news/irans-rial-collapse-mirrors-lebanons-crisis-driving-citizens-to-bitcoin-dab77748-d289-40ae-b5a0-35bbf0d403d1) |

Outside Ukraine, the documented blockade fundraisers are small. The large flows are in crisis economies, and most of them are stablecoins. The need is real and intense for the people involved, but it doesn't add up to a large, steady payment market.

## Key assumptions

1. **Being cut off is what moves people to bitcoin.** Supported by every donation case. Untested: whether they stay.
2. **Readiness matters more than features.** Groups that already had bitcoin set up (WikiLeaks's address, a BTCPay server) received; there's no public evidence on how long setup takes under pressure.
3. **Self-custody is the property that counts.** Supported by Canada and by the custodial exits. Contradicted if self-custodial users get stuck at the edges (app removal, operator refusal, exchange checks).
4. **Stablecoins will keep winning daily use in crises** as long as freezes stay rare for ordinary users.

## What could serve this

**Kinds of product**

- **Wallets** with strong self-custody, no single operator, and a tested exit to the chain.
- **Donation pages** that can't be shut off (self-hosted BTCPay Server, as the Feminist Coalition used).
- **Creator storefronts** with bitcoin checkout, only useful if buyers can pay easily.
- **Preparedness kits:** guides and setup help for groups before they're cut off, like the Human Rights Foundation's "Bitcoin for Nonprofits" guide for groups facing "frozen accounts, blocked wires" ([HRF](https://hrf.org/latest/bitcoin-becomes-lifeline-for-activists-as-hrf-unveils-bitcoin-for-nonprofits-guide/), May 2026).
- **Privacy tools,** which matter as much as censorship resistance for at-risk users.
- **Cash-out networks:** trusted traders who turn bitcoin into local cash, as in Sudan.

## Trade-offs for self-custodial, client-side products

| Property | What helps | What it costs |
| --- | --- | --- |
| No single operator | Multiple servers or providers; unilateral exit | Arkade runs one operator today; exits cost on-chain fees and must happen in time |
| Staying installed | Open source, web app, sideloading | Harder to distribute; fewer users trust it |
| Receiving when cut off | Reusable payment pages, BOLT-12 offers | Lightning needs liquidity and being online, or a service |
| Privacy | Fewer servers that see metadata; Tor | Chain surveillance holds up in court ([Stout](https://www.stout.com/en/insights/article/judicial-scrutiny-chainalysis)); every service in the path sees something |
| Savings | Cold storage, on-chain | Not a payments wallet; carrying a seed phrase works but is fragile |

**Where self-custody genuinely conflicts**

- **Cash-out.** Spending usually means converting at an exchange or trader, where identity checks and freezes return.
- **Developer exposure.** A wallet developer's legal status shapes which countries it can serve; Phoenix and Wallet of Satoshi both left markets, and Phoenix came back to the US only after the Justice Department changed its policy.
- **Platforms:** most of the crisis economies are Android-heavy, where sideloading is possible; iPhone users depend more on the App Store.

## Risks and open questions

**Risks**

- **Reputation and Apple:** being seen as a tool for whatever gets cut off attracts scrutiny.
- **Sanctions:** OFAC's rules apply to wallet providers and users; helping people in sanctioned countries can cross legal lines.
- **Safety:** for activists, a payment app's metadata can be dangerous, so privacy matters as much as censorship resistance.
- **Prosecution:** the line between writing software and running a money transmitting business is policy, not settled law, in the US.

**Open questions**

1. What happens *after* someone is cut off? Which tools do they reach for, how quickly, and do they keep using them?
2. Would creators cut off by card networks use bitcoin payment pages if buyers could pay easily? What stops buyers today?
3. In crisis economies, does anyone use bitcoin for *payments*, or only for savings and leaving?
4. How much does censorship resistance depend on the layer: on-chain, Lightning, Ark with one operator, Ark with many?
5. Does privacy matter more than censorship resistance to activists and at-risk users?

## Research plan: say, do, make

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 5–8 organizers who were cut off (activist groups, creators, nonprofits), through organizations such as HRF | What broke, what they tried, what they still use |
| Case reconstruction | Do | 3 public cases, from first freeze to a year later | Timelines, channels, amounts, what stuck |
| Preparedness test | Make | Small nonprofits setting up to receive bitcoin from scratch | How long it takes, where they get stuck |
| Layer comparison | Do | Wallets on Lightning, Ark, Spark, Fedimint, Cashu | Who can block what, and how exit works in practice |

**Outputs:** a timeline of what happens after being cut off, a setup guide tested with real organizations, and an updated thesis.

*[Open: safety and consent for at-risk participants; how to recruit without exposing them.]*

## Sources

**Context:** [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments) · [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)

**Donations and cut-offs:** [Bitcoin Magazine on the Feminist Coalition](https://bitcoinmagazine.com/culture/nigerian-protest-group-finds-sovereign-lifeline-in-bitcoin) · [CoinDesk on the Feminist Coalition](https://www.coindesk.com/nigerian-activists-bitcoin-endsars-police-brutality/) · [Protos on FBK donations](https://protos.com/alexei-navalny-bitcoin-donations-putin/) · [Moscow Times on Russia's opposition](https://www.themoscowtimes.com/2026/09/10/russian-opposition-finds-refuge-in-bitcoin) · [Elliptic on Ukraine, 2022](https://www.elliptic.co/insights/live-updates-ukraine-government-turns-to-crypto-to-crowdfund-millions-of-dollars) · [Elliptic on Ukraine, 2023](https://elliptic.co/blog/analysis/crypto-donations-to-ukraine-and-russia-breaking-down-the-numbers) · [Christian Science Monitor on WikiLeaks](https://www.csmonitor.com/World/Latest-News-Wires/2011/1024/Wikilieaks-says-financial-blockade-could-put-it-out-of-business) · [Bitcoin Magazine on WikiLeaks](https://bitcoinmagazine.com/culture/wikileaks-public-donation-address-receives-th-bitcoin-1480629241) · [Fortune on the convoy](https://fortune.com/2022/02/18/freedom-convoy-protests-canada-lawsuit-freeze-crypto-wallets-ottawa) · [Federal Court of Appeal, 2026 FCA 6](https://www.fca-caf.ca/en/pages/decisions/plain-language-decision-summaries/2026-fca-6) · [CP24 on the Supreme Court appeal](https://www.cp24.com/news/canada/2026/10/22/supreme-court-to-hear-federal-appeal-over-use-of-emergencies-act/)

**Creators and debanking:** [Notebookcheck on Steam](https://www.notebookcheck.net/Steam-tightens-adult-content-rules-after-pressure-from-payment-giants.1059462.0.html) · [Decrypt on the pressure campaign](https://decrypt.co/332395/pressure-group-forced-steam-remove-adult-games-coming-after-crypto-next) · [Boston Globe on sex workers](https://www.bostonglobe.com/2023/06/01/business/digital-payment-platforms-shutting-out-sex-workers) · [KQED on sex workers and crypto](https://www.kqed.org/news/11899955/when-banks-turned-their-backs-on-them-some-adult-entertainment-workers-turned-to-cryptocurrency) · [Cooley on the debanking executive order](https://www.cooley.com/news/insight/2025/2025-08-14-executive-order-guarantees-efforts-against-debanking-will-continue) · [Sidley on the OCC's debanking report](https://www.sidley.com/en/insights/newsupdates/2026/10/office-of-the-comptroller-of-the-currency-issues-final-report-on-debanking) · [American Banker on Cato's report](https://www.americanbanker.com/news/cato-report-says-administration-misdiagnosed-debanking)

**Crisis economies:** [Chainalysis 2026 adoption index](https://www.chainalysis.com/blog/2026-global-crypto-adoption-index/) · [Chainalysis on Sub-Saharan Africa](https://www.chainalysis.com/blog/subsaharan-africa-crypto-adoption-2025/) · [Pulse on Iran and Lebanon](https://www.pulse.bot/crypto/news/irans-rial-collapse-mirrors-lebanons-crisis-driving-citizens-to-bitcoin-dab77748-d289-40ae-b5a0-35bbf0d403d1) · [Sumsub on Venezuela](https://sumsub.com/media/news/stablecoins-used-in-venezuela-amid-inflation-fears/) · [Elliptic on A7A5](https://www.elliptic.co/insights/the-fall-of-a7a5-how-sanctions-strangled-the-ruble-stablecoin/) · [Elliptic on Myanmar](https://www.elliptic.co/insights/the-digital-kyat-tracing-the-cbdc-financing-over-11-5-million-in-civil-war-donations-to-myanmars-opposition/) · [CNBC on a Ukrainian refugee](https://www.cnbc.com/2022/03/23/ukrainian-flees-to-poland-with-2000-in-bitcoin-on-usb-drive.html) · [Al Jazeera on Lebanon](https://www.aljazeera.com/economy/2020/2/25/distrust-in-lebanese-banks-spurs-bitcoin-boom) · [No Bullshit Bitcoin on Sudan](https://nobsbitcoin.com/how-bitcoin-helps-civilians-escape-the-war-in-sudan) · [The Block on Iran](https://www.theblock.co/post/385941/iran-crypto-ecosystem-irgc-footprint-bitcoin-withdrawals-surge-during-protests-chainalysis) · [Techpoint on Nigeria](https://techpoint.africa/2024/03/04/more-p2p-takes-place-on-whatsapp/) · [Cointelegraph on Afghanistan](https://cointelegraph.com/news/taliban-had-a-massive-chilling-effect-on-afghan-crypto-market-report)

**Layers and chokepoints:** [b10c on missing sanctioned transactions](https://b10c.me/observations/08-missing-sanctioned-transactions/) · [The Block on Wallet of Satoshi](https://www.theblock.co/post/264585/wallet-of-satoshi-bitcoin-lightning) · [The Rage on Wallet of Satoshi in the EU](https://www.therage.co/wallet-of-satoshi-eu-mica/) · [Cointelegraph on Phoenix and Wasabi](https://cointelegraph.com/news/phoenix-wallet-acinq-zksnacks-wasabi-wallet-united-states-crackdown) · [bitcoin.fr on Phoenix's return](https://bitcoin.fr/phoenix-wallet-de-retour-aux-usa/) · [Lightning censorship by network operators (AFT 2024)](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.AFT.2024.12) · [Arkade FAQ](https://docs.arkadeos.com/learn/faq/what-if-the-operator-disappears-or-acts-maliciously) · [Spark docs](https://docs.spark.money/learn/tldr.md) · [Fedimint on trust](https://fedimint.org/users/privacy-and-trust) · [Cashu FAQ](https://docs.cashu.space/faq) · [TechCrunch on Wiper](https://techcrunch.com/?p=1132099) · [Meduza on Apple in Russia](https://meduza.io/en/news/2026/05/25/apple-removed-1-213-apps-at-russia-s-internet-regulator-s-request-in-2025) · [Decrypt on Google Play's rules](https://decrypt.co/335134/google-non-custodial-wallets-exempt-new-crypto-app-rules-play-store) · [DL News on Samourai](https://www.dlnews.com/articles/defi/samourai-dev-gets-max-sentence-for-money-transmission-charge/) · [No Bullshit Bitcoin on Wasabi's coordinator](https://nobsbitcoin.com/zksnacks-to-suspend-its-coinjoin-coordination-service-on-june-1st) · [DOJ memo, April 2025](https://www.justice.gov/dag/media/1395781/dl?inline) · [HRF's Bitcoin for Nonprofits](https://hrf.org/latest/bitcoin-becomes-lifeline-for-activists-as-hrf-unveils-bitcoin-for-nonprofits-guide/) · [Stout on chain analysis in court](https://www.stout.com/en/insights/article/judicial-scrutiny-chainalysis)

**Rules:** [GENIUS Act](https://www.govinfo.gov/content/pkg/PLAW-119publ27/html/PLAW-119publ27.htm) · [FinCEN withdrawal](https://public-inspection.federalregister.gov/2026-20430.pdf) · [EBA on the travel rule](https://www.eba.europa.eu/publications-and-media/press-releases/eba-issues-travel-rule-guidance-tackle-money-laundering-and-terrorist-financing-transfers-funds-and) · [Notabene on self-hosted addresses](https://notabene.id/post/key-takeaways-from-the-ebas-consultation-on-travel-rule-guidelines) · [Didit on the AML Regulation](https://didit.me/blog/amlr-crypto-casp-requirements/) · [FATF targeted update, July 2026](https://fiaumalta.org/app/uploads/2026/07/7th-targeted-update-on-implementation-fatf-standards-vas-vasps-2026.pdf.coredownload.pdf) · [OFAC guidance](https://ofac.treasury.gov/media/913571/download?inline) · [Fifth Circuit on Tornado Cash](https://www.ca5.uscourts.gov/opinions/pub/23/23-50669-CV0.pdf) · [Treasury delisting](https://home.treasury.gov/news/press-releases/sb0057) · [UK SI 2025/688](https://www.legislation.gov.uk/uksi/2025/688/made) · [Proceeds of Crime Act, s.303Z37](https://www.legislation.gov.uk/ukpga/2002/29/section/303Z37)

*Research for this draft was done with AI agents, each claim checked against an opened source; Chainalysis's 2026 figures, FinCEN's withdrawal and the Canadian appeal ruling were rechecked by hand.*
