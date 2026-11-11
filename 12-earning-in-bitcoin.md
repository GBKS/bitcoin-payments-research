# Earning in bitcoin

*Deep dive, first draft. Builds on the November 8 quick scan. Desk research only. Last updated November 11, 2026.*

## Thesis

Almost nobody is paid in bitcoin, so spending it means buying it first. Spiral's summary of the community's input names earning as the strongest lever ([Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)). The evidence below suggests that bitcoin earning, where it exists, is mostly *manufactured*:

- **Conversion services** turn fiat pay into bitcoin, so the payer never touches it.
- **Platforms** pay users small amounts out of ad or marketing budgets.
- **Community projects** create earners on purpose, so local merchants have customers.

Income that people earn in the open market, from clients and employers who choose the rail, goes mostly to stablecoins. Where the goal is dollar income, dollars win.

**The hypothesis:** bitcoin earning grows where three things meet: a **payer who can stay in fiat**, an **earner who wants savings rather than dollar income**, and a **place to spend** some of it. Products that connect those three, rather than asking payers to adopt bitcoin, are where demand could come from.

*Status: a working hypothesis from desk research. Almost none of the evidence on what earners actually do with their bitcoin exists in public; that gap is the main thing direct research would need to fill.*

## What we mean

**Earning in bitcoin:** receiving bitcoin as payment for work, goods, content or attention, as opposed to buying it.

| Kind | Who pays | How bitcoin arrives | Example |
| --- | --- | --- | --- |
| Converted pay | An employer or client, in fiat | A service converts some or all of the pay | Direct deposit through Strike, River, Cash App or Fold; Bitwage |
| Direct pay | A client or employer who holds bitcoin | Invoice or address | Freelancers paid by bitcoin companies; Lightning invoices |
| Platform payouts | A platform, from ad or marketing budgets | Payout to a Lightning address or in-app balance | Bitcoin-rewarding games, Stacker News |
| Social earnings | Many people, in small amounts | Tips, zaps, streaming payments | Nostr zaps, value-for-value podcasts and music |
| Community wages | A community project | Wages or stipends in sats | Afribit Kibera, Bitcoin Ekasi |
| Merchant income | Customers | Payments at the counter | Local shops in circular economies |

Merchant income is covered in [Last-mile infrastructure](18-last-mile-infrastructure.md) and [Landscape](02-landscape.md). Agents earning bitcoin are covered in [Agentic payments](13-agentic-payments.md).

## What people say, and what they do

**Say:** an Oobit survey of 1,004 US full-time employees found 43% want some of their pay in digital assets, and bitcoin was the most preferred asset at 46%, far ahead of stablecoins at 11% ([Bitcoin Magazine](https://bitcoinmagazine.com/news/demand-for-crypto-pay-surges-but-payroll-systems-fall-behind-research), April 2026). *Oobit sells crypto payments, so treat this as directional.*

**Do:**

- **Crypto salaries are stablecoins.** In Pantera's survey of over 1,600 people working in the blockchain industry, 9.6% were paid in crypto, a threefold jump. USDC (63%) and USDT (28.6%) made up over 90% of crypto salaries ([Pantera](https://panteracapital.com/blockchain-compensation-survey-2024/), August 2025).
- **Payroll providers report stablecoin volume.** Over 50% of Rise worker withdrawals are taken in stablecoins ([Rise](https://www.riseworks.io/blog/q3-2026-stablecoin-payroll-report), September 2026). Deel processed $250 million in crypto payouts in 2025, and its 2026 launches are stablecoin salaries ([CPA Practice Advisor](https://www.cpapracticeadvisor.com/2026/05/26/deel-announces-stablecoin-salary-payouts-new-head-of-crypto/183971/), May 2026). Bitwage, the pioneer of bitcoin payroll, now belongs to Paystand and lists "USDC, USDT, BTC, and local currencies" ([Bitwage](https://bitwage.com/en-us/blog/bitwage-joins-paystand), November 2025).
- **Mainstream gig platforms choose stablecoins.** DoorDash will let couriers receive earnings in stablecoins via Stripe's Tempo blockchain ([PaymentsJournal via Pulse](https://www.pulse.bot/fintech/news/doordash-to-offer-gig-workers-stablecoin-payouts-63045324-8b01-4649-ae52-06e4eb92a150/), April 2026). Nigerian gig workers prefer stablecoins to the naira for speed, fewer clawbacks and dollar savings; bitcoin comes up only as "jumpy" ([Nairametrics](https://nairametrics.com/2026/02/24/why-nigerian-gig-workers-prefer-stablecoin-payments-to-the-naira/), February 2026).
- **Bitcoin used to be bigger in payroll.** In a 2022 Deel survey, 47% received some payment in bitcoin, the leading option, ahead of USDC at 29%. The article implies this is among workers who take pay in crypto, not all workers ([Cointelegraph](https://cointelegraph.com/magazine/beyond-the-headlines-the-real-adoption-of-bitcoin-salaries), August 2022). *[to verify: the denominator, against Deel's own report]* Even then, Deel said Latin American workers "often convert it right away into local currency."

**A caution on the comparison:** these are different populations. Oobit asked ordinary employees what they'd like; Pantera asked people already working in crypto what they get. The gap between them is suggestive, not a measured say-do gap for the same people. *(See item 7 in [To do](TODO.md).)*

**What earners do with it:** the only public data is self-reported. Of Oobit's respondents paid in digital assets, 29% converted to dollars immediately, 29% held for a while before converting, 25% still hold all of it and 16% spent it directly; people could pick several answers ([Oobit](https://www.oobit.com/blockchain-payroll)). No provider publishes data on how much bitcoin earners keep, convert or spend.

## Why existing payments serve bitcoin earners badly

The problems are mostly on the payer's side, and in the paperwork:

- **The payer has to hold bitcoin.** Direct pay only works when the client already has bitcoin. A comparison by Spark lists low client adoption alongside BTCPay's setup effort, missing fiat conversion, volatility and tax reporting ([Spark](https://www.spark.money/tools/bitcoin-freelancer-payment-comparison)). *Spark sells a competing product.*
- **Wage law wants cash.** In the US, minimum and overtime wages must be paid "in cash or negotiable instrument payable at par" ([29 CFR 531.27](https://www.law.cornell.edu/cfr/text/29/531.27)). New York City's mayor took his first paycheck in bitcoin and ether in 2022 only by having it converted through Coinbase; the city couldn't pay in crypto directly ([Time](https://time.com/6140923/new-york-city-mayor-adams-cryptocurrency)). Germany's Federal Labor Court allowed crypto as a benefit in kind in 2025, but the part of wages protected from seizure must be paid in money ([Haufe](https://www.haufe.de/recht/arbeits-sozialrecht/bag-kryptowaehrung-als-arbeitsentgelt-ist-zulaessig_218_647236.html)). Brazil's bill PL 957/2025 would allow up to 50% of a salary in crypto ([Cointelegraph](https://cointelegraph.com/news/brazil-bill-bitcoin-salary-regulation), March 2025). *[to verify: current status]*
- **Tax treats it as income, then again as an asset.** In the US, bitcoin wages are taxed at their dollar value on the day of receipt ([IRS](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions)), and spending it later is a taxable disposal. The UK treats crypto received as employment income as "money's worth" ([HMRC](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto21100)). A US exemption for small transactions, Senator Lummis's S.2207 ($300 per transaction, $5,000 a year), was still in committee in August 2026 ([CoinTracking](https://cointracking.info/blog/crypto-de-minimis-tax-exemption)). *[to verify: status since August 2026]* Every small payment an earner spends is a record to keep.
- **Volatility lands on the earner.** Rent and bills are in local currency. That's the main reason earners convert to stablecoins, and why a fixed salary in bitcoin is rare.
- **Custody by default.** The easiest ways to "get paid in bitcoin" in the US hold the bitcoin for the earner (below). Moving it to one's own wallet is an extra step, usually on-chain.

## Case studies

### Converted pay: payroll that never touches bitcoin

The most common way to be "paid in bitcoin" is not to be paid in bitcoin at all. The employer pays in dollars and a service converts.

- **US consumer apps.** River offers to "get paid in bitcoin with zero fees" through direct deposit, with automatic withdrawals to the earner's own wallet ([River](https://river.com/banking)). Cash App charges "zero fees and zero spread" on direct deposits converted to bitcoin ([Cash App](https://cash.app/bitcoin/fees)). Fold's "Direct To Bitcoin" converts up to 100% of deposits; custody is provided by BitGo ([Fold](https://blog.foldapp.com/direct-to-bitcoin/)). Strike sends automatic withdrawals to the earner's own wallet, triggered by direct deposits among other things; "all auto-withdrawals are sent on-chain" ([Strike](https://strike.me/blog/announcing-bitcoin-auto-withdrawals)). A comparison lists Strike as free up to $20,000 a month and River up to $30,000 ([Spark](https://www.spark.money/tools/crypto-paycheck-direct-deposit-comparison)). *[to verify: Strike's own fee page couldn't be opened]*
- **Cross-border payroll.** Bitwage reported over 90,000 workers and 4,500 companies, and over $350 million paid to workers in more than 100 countries ([Bitwage](https://bitwage.com/en-us/blog/bitwage-revolutionizing-the-world-of-remote-work-for-over-10-years/), August 2024), without a split between bitcoin and stablecoins. It paid the first salaries over Lightning in December 2021 ([Bitwage](https://bitwage.com/en-us/blog/bitcoin-lightning-network-payroll)) and describes its bitcoin payroll as sending "to any wallet" ([Bitwage](https://bitwage.com/en-us/blog/bitwage-simplifying-bitcoin-payroll-for-companies-and-employees/), 2023).
- **Employer plans.** When a Texas bank offered staff part of their pay in bitcoin, close to 20% of its 450 employees enrolled; the bank capped it at 10% of each paycheck ([American Banker](https://www.americanbanker.com/news/why-some-banks-and-sports-teams-offer-bitcoin-savings-plans), 2022).
- **Public cases follow the same pattern.** An NFL player took about half of a $13 million salary in bitcoin in 2020; the club paid in dollars and Strike converted ([CNBC](https://www.cnbc.com/2020/12/30/russell-okungs-bitcoin-salary-could-trigger-more-pro-athletes-to-invest.html)).

**What it shows:** "paid in bitcoin" usually means *saving a share of a fiat paycheck automatically*. The bitcoin goes to savings, not to spending, and arrives on-chain or in a custodial account rather than over Lightning. None of these services publishes how many people use it or how much is converted.

### Social earnings: creators, tips and streaming payments

Bitcoin's most native form of earning is small, frequent payments between people.

- **Nostr zaps** (Lightning tips attached to posts on Nostr, an open social protocol). More than 142,000 zaps had been sent by early March 2023, from over 8,000 senders to about 6,000 receivers ([CriptoNoticias](https://criptonoticias.com/tecnologia/ya-enviaron-mas-100000-propinas-bitcoin-nostr)). By August 2026 a community tracker counted 6.99 million zaps worth 43.32 BTC in total, from 180,000 senders, growing by about 20,000 zaps a week ([Nostr Recap](https://njump.me/4a49af9d61d96fc6fad0cde5465164e8bd76944f59d60fc1b9e32a65a111fb9c)). *Totals depend on which relays a tracker indexes.*
- **Value-for-value podcasting.** Listeners on Fountain sent $127,900 to creators in 2024, including over 40,000 "boosts" (payments with a message) averaging 3,380 sats ([Fountain via Stacker News](https://stacker.news/items/829867)). A podcasting educator reported about 100,000 sats earned without promoting it ([The Audacity to Podcast](https://theaudacitytopodcast.com/?p=31616), 2023).
- **Music.** Wavlake grew to over 480 artists by December 2023 ([Wavlake](https://zine.wavlake.com/2023-year-in-review/)); its first track to earn 1 million sats was worth over $700 ([Podnews](https://podnews.net/press-release/wavlake-zbd), 2024). Wavlake pays straight to the artist's own Lightning address.
- **Stacker News** (a forum that pays in sats). In September 2025, 583 users wrote posts and comments and earned 2,688,420 sats in zaps between them ([Stacker News](https://stacker.news/items/1246185)).

**What it shows:** a working culture of earning, but small. All the zaps ever counted add up to about 43 BTC. The earners and payers are mostly the same community, and sats circulate inside it: a podcast app's boost bot is among the top zap recipients ([Nostr Recap](https://njump.me/4a49af9d61d96fc6fad0cde5465164e8bd76944f59d60fc1b9e32a65a111fb9c)). No public evidence shows creators outside bitcoin circles choosing sats at scale.

### Platform payouts: games and rewards

- **Bitcoin-rewarding games.** ZBD's SDK pays players from ad revenue converted to bitcoin; its game Idle Bank passed 12 million downloads ([Bitcoin Magazine](https://bitcoinmagazine.com/business/zbds-sdk-powers-bitcoin-earnings-in-mobile-games-driving-124-revenue-growth), September 2025). ZBD raised $40 million in January 2026, worked with 55 games in 2025, and "centers its technology on Bitcoin rather than stablecoins" ([Bitcoin Magazine](https://bitcoinmagazine.com/news/bitcoin-payments-startup-zbd-raises-40m)). A ZBD-powered game, Bitcoin Miner, reports over 20 million downloads and over $3.7 million paid to players ([Spark](https://www.spark.money/tools/bitcoin-gaming-platform-comparison)). *Company figures, via a competitor's comparison page.*
- **Attitudes, not use:** in ZBD's own study of 2,000 US Gen Z gamers, 74% said they'd be more receptive to ads if rewarded in bitcoin ([PR Newswire](https://prnewswire.com/news-releases/the-zbd-gen-z-gamer-study-goes-live-wtf-does-gen-z-think-of-gaming-brands-and-bitcoin-302145396.html), 2024).
- **Sats-back rewards.** Cards and apps such as Fold pay rewards in bitcoin on spending. Custodial; covered in [Payments that feel different](16-payments-that-feel-different.md) as a game-like mechanic.

- **Task marketplaces.** Spiral names Trails Coffee and BitTasker as live projects where people earn bitcoin ([Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)). BitTasker is a Nostr-based task marketplace for Android and web ([Rootstock docs](https://dev.rootstock.io/dev-tools/wallets/bittasker/)). *[to verify: couldn't open either project's site, so what Trails Coffee does and how BitTasker pays are unconfirmed]*

**What it shows:** platforms can create millions of small bitcoin earners cheaply, because the payer is an advertiser. This is the largest reach of any form of bitcoin earning, at the smallest amounts per person.

### Community wages: circular economies

Several projects pay people in bitcoin on purpose, so that local merchants have customers who hold it.

- **Afribit Kibera (Nairobi, Kenya).** The project reports over 2,600 residents who adopted bitcoin, with about 60 merchants and nearly 100 garbage collectors paid in bitcoin ([Business Daily](https://www.businessdailyafrica.com/bd/markets/currencies/bitcoin-revolution-steadily-shaping-trade-in-kibera-5307718), December 2025). A later report puts active users at "400–600+ active users with real transactions," with the lessons "Trust first, Bitcoin second" and "Create earners before merchants" ([Blink](https://blink.sv/blog/weekly-brief-2026-19), May 2026).
- **Bitcoin Ekasi (Mossel Bay, South Africa).** Coaches and lifeguards were paid their full salary in bitcoin, at about $150 a month for junior coaches ([Bitcoin Magazine](https://bitcoinmagazine.com/culture/bitcoin-ekasi-township-one-year-later), 2022). Over 57 shops accept it ([Blink](https://www.blink.sv/blog/weekly-brief-50-2025), December 2025).
- **Bitcoin Jungle (Costa Rica).** Over 380 locations accepted bitcoin by mid-2024; early on, 30–40% of vendors cashed out daily or at weekends ([Bitcoin News](https://bitcoinnews.com/p/bitcoin-jungle-richard-scotford), 2025).
- **A local loop in Kenya.** A worker paid in bitcoin by a European employer through Blink pays his internet bill with it, because his provider accepts Blink too ([Blink](https://blink.sv/blog/bitcoin-lightning-payments-europe-to-kenya-with-blink-eu), 2024). Since May 2026, every M-Pesa number in Kenya can receive Lightning payments through Tando: unclaimed numbers get shillings (1% fee), and claimed ones keep bitcoin ([Blink](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address)). Tando processed over 100 transactions a day by mid-2025 ([Crypto Briefing](https://cryptobriefing.com/bitcoin-lightning-payments-kenya-tando/)).

**What it shows:** earning comes first. The projects that last start by creating earners, then merchants follow. The gap between "adopted" (2,600) and active (400–600) in Kibera is the say-versus-do gap in miniature. These loops are small, subsidized at the start, and depend on a few organizers.

### El Salvador: a warning about mandates

El Salvador made bitcoin legal tender in 2021 and amended the law in January 2025 under an IMF deal: acceptance is now optional, taxes can't be paid in bitcoin, and the state wallet Chivo is being wound down ([Decrypt](https://decrypt.co/303626/el-salvador-bitcoin-law-amendment-imf-loan)).

- Only 8.1% of Salvadorans used bitcoin to pay in 2024, the lowest since 2021, in a poll of 1,266 people by the Central American University's IUDOP ([El Heraldo](https://www.elheraldo.hn/mundo/uso-del-bitcoin-salvador-alcanza-nivel-mas-bajo-2024-CF23621470), January 2025).
- An independent face-to-face survey of 1,800 households in February 2022 found that 20% of respondents kept using Chivo after spending its $30 sign-up bonus. Only 20% of firms accepted bitcoin, bitcoin made up 4.9% of sales on average, and 88% of businesses converted their bitcoin sales to dollars ([Alvarez, Argente and Van Patten](https://www.davidargente.com/_files/ugd/b05023_7825615207654784864b4c4cc4ec6550.pdf), April 2022; also reported by [The Block](https://www.theblock.co/post/144927/everyday-bitcoin-usage-in-el-salvador-remains-low-despite-government-push-us-academic-study-finds)).
- At El Zonte ("Bitcoin Beach"), a 2026 report says bitcoin payments have become rare and most transactions are by card ([Crypto Briefing](https://cryptobriefing.com/bitcoin-usage-declines-in-el-zonte-as-card-payments-rise/), August 2026), while the tourism minister claims sales there rose 30% thanks to bitcoin, without data ([El Salvador in English](https://elsalvadorinenglish.com/2025/11/11/el-salvadors-bitcoin-beach-sees-30-sales-growth/), November 2025).

**What it shows:** a mandate and a bonus didn't create earners. I found no 2025–2026 source on salaries paid in bitcoin there. *[to verify]*

### Freelancers in Africa and Latin America: buying versus being paid

- **Nigeria and South Africa buy bitcoin.** On centralized exchanges, bitcoin is 89% of crypto purchases with naira and 74% with rand, against 51% in dollar markets; USDT is 7% in Nigeria ([Chainalysis](https://www.chainalysis.com/blog/subsaharan-africa-crypto-adoption-2025/), September 2025). The data excludes informal, peer-to-peer and business-to-business transfers, where stablecoins dominate trade flows.
- **Argentina buys dollars and holds bitcoin.** On Bitso in the first half of 2025, stablecoins were 85% of purchases and bitcoin 4%, yet bitcoin was in 55% of wallets ([Mercado](https://mercado.com.ar/tendencias/bitso-stablecoins-dominan-compra-y-bitcoin-crece-en-carteras-durante-2025), August 2025). Bitwage's founder says Argentine freelancers exporting services are already paid in stablecoins ([iProfesional](https://www.iprofesional.com/economia/426669-fin-cepo-revelan-que-stablecoins-ganan-terreno-entre-freelancers-empresas), April 2025).
- **Latin America overall** leans to stablecoins: they were over half of exchange purchases with pesos and reais ([Chainalysis](https://www.chainalysis.com/blog/latin-america-crypto-adoption-2025/), October 2025).

**What it shows:** people *buy* bitcoin to save, and get *paid* in dollars to live. No public source shows a group of market earners choosing bitcoin over stablecoins as income.

## Lessons from elsewhere

How people treat money earned in a separate currency, from games, gig work and research on mental accounting:

- **Earned platform money gets cashed out, but nobody publishes how much is kept.** Roblox creators earned $1.5 billion in 2025 through its cash-out program, and "do not always seek to receive fiat currency payouts" ([Roblox 10-K](https://www.sec.gov/Archives/edgar/data/1315098/000131509826000024/rblx-20251231.htm)). Cash-out requires at least 30,000 earned Robux ([Roblox](https://create.roblox.com/docs/production/monetization/developer-exchange)). The share kept is the same missing number as for bitcoin earners.
- **Earners pay to get their money sooner.** In 2022, 7.2 million US workers used employer-linked early-pay products, and 96.6% of their fees were for faster access ([CFPB](https://www.consumerfinance.gov/data-research/research-reports/data-spotlight-developments-in-the-paycheck-advance-market/), 2024). More than half of Lyft drivers used its instant cash-out, by Stripe's account ([Stripe](https://stripe.com/ie/newsroom/stories/lyft-and-stripe), 2017). For people living on their income, liquidity beats the form of payment.
- **How money is framed changes how it's spent.** People given $25 described as a "bonus" spent far more of it than those given the same amount as a "rebate" ([Phys.org on Epley, Mak and Idson](https://phys.org/news/2008-02-tax-rebates-bonuses.html)). Loyalty points are hoarded: about a third go unredeemed, and in one retail panel only 3% of purchases used points ([Advanced Management on Stourm et al.](https://advancedmanagement.net/perspectives/2017/08/why-consumers-stockpile-rather-spend-loyalty-program-points)). Gift cards go unspent too: 47% of US adults hold at least one ([PBS](https://www.pbs.org/newshour/economy/forget-to-spend-an-old-gift-card-heres-what-happens-to-that-money)).
- **Big numbers make people underspend.** When a foreign currency's face value is a multiple of the home currency, people value products closer to the number on the note ([Raghubir and Srivastava](https://econpapers.repec.org/RePEc:oup:jconrs:v:29:y:2002:i:3:p:335-47), 2002). Amounts in sats might have the same effect *[assumption: untested for bitcoin]*.

## Sizing

Nobody publishes how much income is paid in bitcoin. The visible pieces, side by side:

| Flow | Size | Source |
| --- | --- | --- |
| Nostr zaps, all time to August 2026 | 6.99 million zaps, 43.32 BTC | [Nostr Recap](https://njump.me/4a49af9d61d96fc6fad0cde5465164e8bd76944f59d60fc1b9e32a65a111fb9c) |
| Fountain listeners to creators, 2024 | $127,900 | [Stacker News](https://stacker.news/items/829867) |
| Stacker News zaps to users, September 2025 | 2.69 million sats, 583 users | [Stacker News](https://stacker.news/items/1246185) |
| Bitcoin Miner game payouts, lifetime | over $3.7 million (company claim) | [Spark](https://www.spark.money/tools/bitcoin-gaming-platform-comparison) |
| Kibera active users | 400–600 | [Blink](https://blink.sv/blog/weekly-brief-2026-19) |
| Converted pay (Strike, River, Cash App, Fold) | Not published | |
| **For comparison:** Deel crypto payouts, 2025 | $250 million | [CPA Practice Advisor](https://www.cpapracticeadvisor.com/2026/05/26/deel-announces-stablecoin-salary-payouts-new-head-of-crypto/183971/) |
| **For comparison:** Tempo stablecoin transfers | over $1 billion in 30 days | [Crypto Briefing](https://cryptobriefing.com/tempo-1b-stablecoin-transfer-volume/), September 2026 |

The bitcoin-native flows that can be counted are tiny next to stablecoin payroll. The one flow that might be large, converted pay through US consumer apps, is unpublished. That makes it the most important unknown in this area.

**A bottom-up estimate for converted pay:**

Annual bitcoin bought from paychecks = users with direct deposit to bitcoin × average deposit converted × pay periods per year

Purely as an illustration: 200,000 users × $150 per paycheck × 26 paychecks = $780 million a year. *[assumption: every input is illustrative, not data]* Even at that scale it's savings, not spending: the bitcoin rarely comes back out as payments.

## Key assumptions

What has to be true for the thesis to hold:

1. **Earners want bitcoin as savings, not as income to live on.** Supported by Argentina (hold bitcoin, buy dollars) and by how converted pay is used. Contradicted if earners in a local loop keep all their income in bitcoin.
2. **Payers won't adopt bitcoin, so conversion is the unlock.** Supported by every public case. Contradicted if a meaningful group of clients pays freelancers in bitcoin by choice.
3. **A place to spend matters.** Supported by the circular economies and the Kenyan internet bill. Unclear whether spending creates more earners, or earners create spending.
4. **Self-custodial delivery is wanted.** Unclear. Strike and River offer it, but nobody publishes how many earners use it.

## What could serve this

**Kinds of product**

- **Conversion payroll with self-custodial delivery:** the payer pays fiat, the earner receives a chosen share in bitcoin, to their own wallet.
- **Payout rails for platforms:** APIs that push payments to any Lightning address. Strike, ZBD, OpenNode and Speed offer this ([Strike](https://docs.strike.me/walkthrough/sending-payments/), [ZBD](https://docs.zbdpay.com/payments/payouts/lightning-address), [OpenNode](https://opennode.com/payouts/), [Speed](https://apidocs.tryspeed.com/reference/create-a-instant-send)); Voltage offers credit lines so businesses can pay out over Lightning without pre-funding ([Voltage](https://voltage.cloud/blog/voltage-payments-on-mainnet-credit-backed-lightning-payments-are-live), October 2025).
- **Wallets designed for receiving:** a reusable address, invoices, notes, export, and the fiat value at receipt for tax.
- **Income splitting:** keep a share in bitcoin, send the rest to local money or a stablecoin, automatically.
- **Local loop tools:** merchant acceptance and bridges such as Tando, so earned bitcoin can be spent where the earner lives.
- **Creator tools:** payment pages, tip links and value-for-value integrations that work with any Lightning wallet.

## Trade-offs for self-custodial, client-side products

Receiving is the natural fit for a self-custodial wallet; the hard parts are being reachable and keeping records.

| Feature | Self-custody | Without your own server | How |
| --- | --- | --- | --- |
| Receiving converted pay | Fully | Fully | The conversion service sends on-chain to the earner's address; fees make small amounts expensive |
| A Lightning address for payouts | Fully | Needs a service | A `user@domain` address is resolved by a server at that domain ([LUD-16](https://github.com/lnurl/luds/blob/luds/16.md)) |
| Receiving while the phone is offline | Partly | Needs a service | Phone-based Lightning wallets must be online to receive; Ark and similar layers, or a service, can hold payments for later *[from memory; to verify]* |
| Reusable payment requests | Fully | Fully | BOLT-12 offers; recurring payments are not standardized yet: the recurrence proposal is still a draft ([BOLT 12](https://github.com/lightning/bolts/blob/master/12-offer-encoding.md), [pull request](https://github.com/lightning/bolts/pull/1240)) |
| Tax records | Fully | Fully | Store the fiat value at the time of each receipt and spend on the device; export for tax software |
| Pulling a payout (withdraw links) | Fully | Fully | LNURL-withdraw: the earner scans a code with their own wallet ([OpenNode](https://developers.opennode.com/docs/generate-lnurl-withdrawal)) |
| Income splitting into local money | Partly | Needs a provider | Converting to fiat or stablecoins needs a regulated partner or a swap |

**Where self-custody genuinely conflicts**

- **Conversion is regulated.** Turning a paycheck into bitcoin requires a licensed provider. A wallet can integrate one but not be one.
- **Being reachable.** Platform payouts assume the earner can always receive. A phone that's off can't, unless something holds the payment.
- **Amounts.** Salaries are larger than everyday payments. Payment-focused wallets suit the spending share; the savings share may belong in a savings wallet or cold storage.

**Platform:** converted pay is a US phenomenon, where iOS and Android are both common. Earners in African and Latin American local loops mostly use Android. *[from memory; see item 8 in [To do](TODO.md)]*

## Risks and open questions

**Risks**

- **Tax:** receiving is income and spending is a disposal in most countries, so every small payment is a record.
- **Labor law:** minimum wages must be paid in money in the US and, for the protected part, in Germany. Bitcoin pay is an add-on, not a replacement.
- **Volatility:** the main reason earners convert. Fixed-price obligations sit badly with a bitcoin balance.
- **Dependence on subsidies:** circular economies and rewarding games both rely on someone funding the first earners.
- **Mandates backfire:** El Salvador shows that pushing bitcoin from the top doesn't create lasting use.

**Open questions**

1. Of people who route pay into bitcoin, how much do they keep, spend or move to their own wallet? (The single most useful number; only providers have it.)
2. Are there market earners, not community projects, who choose bitcoin over stablecoins for income? Where, and why?
3. In local loops, what share of earned sats is spent locally versus cashed out? Does that change over time?
4. Do creators earning sats spend them inside the community (zaps, boosts) or cash out?
5. How does this overlap with community-driven economies: fan artists, commissions and group order managers getting paid ([Community-driven economies](11-community-driven-economies.md))?
6. Would a US de minimis exemption change earners' behavior, or only reduce paperwork?

## Research plan: say, do, make

Following Liz Sanders' framework, weighting what people **do** and **make** over what they **say** (see [Method](01-method.md)).

**First target: earners in a local loop.** It's the only place where earning, holding and spending in bitcoin all happen, and the organizers publish what they learn.

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 10 earners and 3 organizers in one circular economy | Why they accept bitcoin, what they do with it, what they'd change |
| Earning diaries | Do | 5–10 earners, for four weeks | Every receipt, spend and cash-out, in their own words |
| Following payouts | Do | One organizer's payroll run, end to end | Where conversion, fees and delays happen |
| Workaround teardown | Make | Earners' notes, spreadsheets, cash-out routines | What they built to cope with volatility and records |
| Public data | Do | Nostr zaps and value-for-value payments | Who earns, how concentrated, how much flows back out |
| Desk research | Say / do | Payroll and payout providers | Published figures; requests for anonymized aggregates |

**Second wave:** people in the US who route part of their pay into bitcoin, recruited without mentioning a product, to answer open question 1.

**Outputs:** a public write-up per wave, a money-flow map of one local loop, and an updated thesis.

*[Open: which circular economy, consent and compensation for diaries, and whether to work with organizers as research partners.]*

## Sources

**Context:** [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)

**Say and do:** [Bitcoin Magazine on the Oobit survey](https://bitcoinmagazine.com/news/demand-for-crypto-pay-surges-but-payroll-systems-fall-behind-research) · [Oobit on blockchain payroll](https://www.oobit.com/blockchain-payroll) · [Pantera's compensation survey](https://panteracapital.com/blockchain-compensation-survey-2024/) · [Rise payroll report](https://www.riseworks.io/blog/q3-2026-stablecoin-payroll-report) · [CPA Practice Advisor on Deel](https://www.cpapracticeadvisor.com/2026/05/26/deel-announces-stablecoin-salary-payouts-new-head-of-crypto/183971/) · [Bitwage joins Paystand](https://bitwage.com/en-us/blog/bitwage-joins-paystand) · [Pulse on DoorDash](https://www.pulse.bot/fintech/news/doordash-to-offer-gig-workers-stablecoin-payouts-63045324-8b01-4649-ae52-06e4eb92a150/) · [Nairametrics on Nigerian gig workers](https://nairametrics.com/2026/02/24/why-nigerian-gig-workers-prefer-stablecoin-payments-to-the-naira/) · [Cointelegraph on bitcoin salaries](https://cointelegraph.com/magazine/beyond-the-headlines-the-real-adoption-of-bitcoin-salaries)

**Rules and tax:** [29 CFR 531.27](https://www.law.cornell.edu/cfr/text/29/531.27) · [IRS virtual currency FAQ](https://www.irs.gov/individuals/international-taxpayers/frequently-asked-questions-on-virtual-currency-transactions) · [HMRC Cryptoassets Manual](https://www.gov.uk/hmrc-internal-manuals/cryptoassets-manual/crypto21100) · [Haufe on the Federal Labor Court ruling](https://www.haufe.de/recht/arbeits-sozialrecht/bag-kryptowaehrung-als-arbeitsentgelt-ist-zulaessig_218_647236.html) · [Cointelegraph on Brazil's bill](https://cointelegraph.com/news/brazil-bill-bitcoin-salary-regulation) · [CoinTracking on de minimis proposals](https://cointracking.info/blog/crypto-de-minimis-tax-exemption) · [Time on New York City's mayor](https://time.com/6140923/new-york-city-mayor-adams-cryptocurrency)

**Converted pay:** [River](https://river.com/banking) · [Cash App fees](https://cash.app/bitcoin/fees) · [Fold: Direct To Bitcoin](https://blog.foldapp.com/direct-to-bitcoin/) · [Strike auto-withdrawals](https://strike.me/blog/announcing-bitcoin-auto-withdrawals) · [Spark's direct deposit comparison](https://www.spark.money/tools/crypto-paycheck-direct-deposit-comparison) · [Bitwage at ten years](https://bitwage.com/en-us/blog/bitwage-revolutionizing-the-world-of-remote-work-for-over-10-years/) · [Bitwage on Lightning payroll](https://bitwage.com/en-us/blog/bitcoin-lightning-network-payroll) · [Bitwage on bitcoin payroll](https://bitwage.com/en-us/blog/bitwage-simplifying-bitcoin-payroll-for-companies-and-employees/) · [American Banker on bitcoin savings plans](https://www.americanbanker.com/news/why-some-banks-and-sports-teams-offer-bitcoin-savings-plans) · [CNBC on a bitcoin salary](https://www.cnbc.com/2020/12/30/russell-okungs-bitcoin-salary-could-trigger-more-pro-athletes-to-invest.html) · [Spark's freelancer payment comparison](https://www.spark.money/tools/bitcoin-freelancer-payment-comparison)

**Social earnings and platforms:** [CriptoNoticias on early zaps](https://criptonoticias.com/tecnologia/ya-enviaron-mas-100000-propinas-bitcoin-nostr) · [Nostr Recap, August 2026](https://njump.me/4a49af9d61d96fc6fad0cde5465164e8bd76944f59d60fc1b9e32a65a111fb9c) · [Fountain's 2024 review](https://stacker.news/items/829867) · [The Audacity to Podcast](https://theaudacitytopodcast.com/?p=31616) · [Wavlake 2023 review](https://zine.wavlake.com/2023-year-in-review/) · [Podnews on Wavlake and ZBD](https://podnews.net/press-release/wavlake-zbd) · [Stacker News monthly stats](https://stacker.news/items/1246185) · [Bitcoin Magazine on ZBD's SDK](https://bitcoinmagazine.com/business/zbds-sdk-powers-bitcoin-earnings-in-mobile-games-driving-124-revenue-growth) · [Bitcoin Magazine on ZBD's raise](https://bitcoinmagazine.com/news/bitcoin-payments-startup-zbd-raises-40m) · [Spark's gaming comparison](https://www.spark.money/tools/bitcoin-gaming-platform-comparison) · [ZBD's Gen Z study](https://prnewswire.com/news-releases/the-zbd-gen-z-gamer-study-goes-live-wtf-does-gen-z-think-of-gaming-brands-and-bitcoin-302145396.html)

**Local loops:** [Business Daily on Kibera](https://www.businessdailyafrica.com/bd/markets/currencies/bitcoin-revolution-steadily-shaping-trade-in-kibera-5307718) · [Blink weekly brief, May 2026](https://blink.sv/blog/weekly-brief-2026-19) · [Blink weekly brief, December 2025](https://www.blink.sv/blog/weekly-brief-50-2025) · [Bitcoin Magazine on Bitcoin Ekasi](https://bitcoinmagazine.com/culture/bitcoin-ekasi-township-one-year-later) · [Bitcoin News on Bitcoin Jungle](https://bitcoinnews.com/p/bitcoin-jungle-richard-scotford) · [Blink: payments from Europe to Kenya](https://blink.sv/blog/bitcoin-lightning-payments-europe-to-kenya-with-blink-eu) · [Blink: M-Pesa numbers as Lightning addresses](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address) · [Crypto Briefing on Tando](https://cryptobriefing.com/bitcoin-lightning-payments-kenya-tando/)

**El Salvador:** [Decrypt on the law amendment](https://decrypt.co/303626/el-salvador-bitcoin-law-amendment-imf-loan) · [El Heraldo on the IUDOP poll](https://www.elheraldo.hn/mundo/uso-del-bitcoin-salvador-alcanza-nivel-mas-bajo-2024-CF23621470) · [Alvarez, Argente and Van Patten: Bitcoin as legal tender in El Salvador](https://www.davidargente.com/_files/ugd/b05023_7825615207654784864b4c4cc4ec6550.pdf) · [The Block on the household study](https://www.theblock.co/post/144927/everyday-bitcoin-usage-in-el-salvador-remains-low-despite-government-push-us-academic-study-finds) · [Crypto Briefing on El Zonte](https://cryptobriefing.com/bitcoin-usage-declines-in-el-zonte-as-card-payments-rise/) · [El Salvador in English on El Zonte](https://elsalvadorinenglish.com/2025/11/11/el-salvadors-bitcoin-beach-sees-30-sales-growth/)

**Africa and Latin America:** [Chainalysis on Sub-Saharan Africa](https://www.chainalysis.com/blog/subsaharan-africa-crypto-adoption-2025/) · [Chainalysis on Latin America](https://www.chainalysis.com/blog/latin-america-crypto-adoption-2025/) · [Mercado on Bitso's data](https://mercado.com.ar/tendencias/bitso-stablecoins-dominan-compra-y-bitcoin-crece-en-carteras-durante-2025) · [iProfesional on Argentine freelancers](https://www.iprofesional.com/economia/426669-fin-cepo-revelan-que-stablecoins-ganan-terreno-entre-freelancers-empresas)

**Payout rails:** [Strike API](https://docs.strike.me/walkthrough/sending-payments/) · [ZBD payouts](https://docs.zbdpay.com/payments/payouts/lightning-address) · [OpenNode payouts](https://opennode.com/payouts/) · [OpenNode LNURL-withdraw](https://developers.opennode.com/docs/generate-lnurl-withdrawal) · [Speed API](https://apidocs.tryspeed.com/reference/create-a-instant-send) · [Voltage Payments](https://voltage.cloud/blog/voltage-payments-on-mainnet-credit-backed-lightning-payments-are-live) · [Lightning Address (LUD-16)](https://github.com/lnurl/luds/blob/luds/16.md) · [BOLT 12](https://github.com/lightning/bolts/blob/master/12-offer-encoding.md) · [BOLT 12 recurrence proposal](https://github.com/lightning/bolts/pull/1240) · [Crypto Briefing on Tempo](https://cryptobriefing.com/tempo-1b-stablecoin-transfer-volume/)

*Research for this draft was done with AI agents, each claim checked against an opened source; three key figures were rechecked by hand. Spark's comparison pages are cited several times; Spark sells a competing product (see item 6 in [To do](TODO.md)).*
