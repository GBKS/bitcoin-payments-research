# Last-mile infrastructure

*Deep dive, first draft. Supporting area. Builds on the November 8 quick scan. Desk research only. Last updated November 10, 2026.*

## Thesis

Most of the people in the other areas need to get money in and out of bitcoin, or pay someone who doesn't use it: a supplier who takes M-Pesa or Pix, a merchant who wants USDT, a shop in Seoul that only takes won. The evidence below suggests four things about that "last mile":

- **It's being built country by country, by small providers.** Kenya, South Africa, Mexico, the Philippines and the EU each have a bridge from Lightning to local money; Korea, as far as this research found, has none.
- **The recipient almost always gets local money.** Kenya's claimed phone numbers and a few merchants who choose to hold bitcoin are the exceptions.
- **Non-custodial doesn't mean always available.** Boltz, the main swap service between bitcoin layers, never held user funds, yet it has been offline since August 2026. Atomic designs limit what an operator can take, not whether it keeps running.
- **Rules are arriving at the edges.** Kenya, Brazil, the EU and South Africa now license conversion services, and several require identifying who owns a self-custody wallet on the other side.

**The hypothesis:** for a self-custodial wallet, the last mile is less about any single integration than about **reach** (paying any local recipient by phone number or QR code), **choice** (more than one provider for each conversion), and **resilience** (still working when one provider exits).

*Status: a supporting area, researched as a reference map. Usage figures for almost every service are missing; the services publish launches, not volumes.*

## What we mean

| Direction | What happens | Example |
| --- | --- | --- |
| Paying out to local systems | A bitcoin payment arrives as local money | Lightning to M-Pesa (Kenya), to SPEI (Mexico), to a bank (EU) |
| Taking in from local systems | Local money arrives as bitcoin or a local token | Pix to DePix (Brazil) |
| Swapping between layers and assets | Moving between on-chain, Lightning, Liquid, Ark, Spark, stablecoins | Boltz, Arkade's solver, Bark's gateway |
| Getting in and out | Buying or selling bitcoin | Peer-to-peer exchanges, apps, ATMs |

## What people say, and what they do

**Say:** the ecosystem says "stay bitcoin-only," and merchants are told to keep the bitcoin they receive.

**Do:** working last-mile services convert at the edge, usually into local money: Tando into shillings, MoneyBadger into rand, DePix into a real-pegged token, Square into dollars by default. Steak 'n Shake, which keeps the bitcoin it receives in a reserve, is the visible exception ([Cointelegraph](https://cointelegraph.com/news/steak-n-shake-bitcoin-accumulation-strategic-reserve-btc-payments), January 2026). Even when the law required acceptance, merchants converted: in El Salvador in February 2022, 88% of businesses turned their bitcoin sales into dollars, and bitcoin made up 4.9% of sales on average ([Alvarez, Argente and Van Patten](https://www.davidargente.com/_files/ugd/b05023_7825615207654784864b4c4cc4ec6550.pdf), a survey of 1,800 households). Where conversion is invisible to the user, people don't seem to mind which rail runs underneath.

**Reach versus use:** Tando makes 40 million M-Pesa numbers reachable; MoneyBadger connects to networks with over 650,000 outlets; Square enabled about 1 million merchants. None publishes how many payments actually arrive.

## By country

| Country | Bridge | How it works | Recipient gets | Usage published |
| --- | --- | --- | --- | --- |
| Kenya | Tando | Every M-Pesa number is a Lightning address; 1% to convert; KES 15–10,000 per payment | Shillings, or bitcoin if the number is claimed | Over 100 transactions a day by mid-2025 |
| South Africa | MoneyBadger | Lightning payments through retail payment networks (Pick n Pay, Engen) | Rand, next business day | About R1.4 million a month (2025) |
| Nigeria | Tapnob; Bitnob | A Lightning address linked to a naira bank account; bank payouts | Naira | None |
| Brazil | DePix | Pix payments settle as a real-pegged token on Liquid | DePix | About half of Liquid's transactions (Q1 2026) |
| Mexico | Bull Bitcoin; Aureo | Peso transfers by SPEI from a self-custodial wallet; Lightning to SPEI | Pesos | None |
| Philippines | Pouch; Coins.ph | Lightning to merchant QR codes; bitcoin at QR Ph merchants (custodial) | Pesos | 400+ merchants (2023) |
| Japan | Aurora | Foreign customers pay Japanese merchants over Lightning | Unclear | None |
| EU | Bringin | Self-custodial Lightning wallet with a personal IBAN, SEPA Instant | Euros or bitcoin | None |
| US | Square | Bitcoin on by default for eligible sellers | Dollars by default, or bitcoin | About 1 million merchants enabled |
| South Korea | None found | — | — | — |

Sources: Kenya ([Blink](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address), [Crypto Briefing](https://cryptobriefing.com/bitcoin-lightning-payments-kenya-tando/)); South Africa ([TechCentral](https://techcentral.co.za/bitcoin-payments-mainstream-south-africa/267462/), [Daba Finance](https://www.dabafinance.com/en/news/moneybadger-crypto-payments-south-africa-bitcoin-retail-adoption), [Blink](https://blink.sv/blog/weekly-brief-2026-15)); Nigeria ([Technext](https://technext24.com/crypto/tapnob-nigeria-crypto-to-naira-gateway/), [Bitnob docs](https://bitnob.dev/docs/payouts/corridor-specific-behavior/nigeria-payout)); Brazil ([BTCPay Server](https://blog.btcpayserver.org/depix-plugin/), [Liquid](https://blog.liquid.net/liquid-federation-quarterly-update-q1-2026/)); Mexico ([Bull Bitcoin](https://bullbitcoin.com/blog/how-to-pay-with-bitcoin-at-any-business-in-mexico), [FinanzWire](https://www.finanzwire.com/press-release/amboss-and-aureo-connect-the-lightning-network-to-mexicos-banking-system-XezkkOlnWrx), a paid press release); Philippines ([Bitcoin Magazine](https://bitcoinmagazine.com/business/400-small-businesses-in-the-philippines-are-now-accepting-bitcoin), [Bitcoin.com News](https://news.bitcoin.com/coins-ph-adds-bitcoin-and-ethereum-to-national-qr-ph-reaching-700000-philippine-merchants/)); Japan ([Bitcoin Magazine](https://bitcoinmagazine.com/news/japanese-bitcoin-industry-unveils-aurora)); EU ([Bringin](https://bringin.app/)); US ([Bitcoin Magazine](https://bitcoinmagazine.com/news/square-crosses-1-million-bitcoin-merchants)). All figures are the companies' own.

**Gaps that matter for the other areas:** no route from Lightning to Korean won was found, which is the currency K-pop group orders settle in ([Community-driven economies](11-community-driven-economies.md)) *[to verify]*. In Brazil, paying a Pix key from a Lightning wallet exists only as a hackathon prototype ([NostrPIX](https://www.btcplusplus.dev/floripa/hackathon/projects/74350840-a01a-4a79-9cb4-8b756373ecf1)); in Argentina, no live service pays any interoperable QR code from Lightning.

## Case studies

### Kenya: phone numbers as payment addresses

Since May 22, 2026, every Kenyan M-Pesa number works as a Lightning address (`phonenumber@bitcoin.co.ke`) through Tando. Payments to unclaimed numbers are converted to shillings and paid out via M-Pesa for a 1% fee; the announcement doesn't say who holds the bitcoin before conversion. Numbers whose owners have claimed them (a one-time KES 210) receive bitcoin directly to their own wallet, with no fee; for those, "The platform never holds your Bitcoin" ([Blink](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address)). This is close to what the [Pave](https://gbks.substack.com/p/pave-protocol-for-last-mile-bitcoin) sketch proposes, built for one country and one provider.

**What it shows:** a wallet that can pay a Lightning address can pay any M-Pesa number with no extra integration. Whether recipients claim their numbers, and keep bitcoin, is unknown: no figures have been published since launch.

### South Africa: bitcoin at the counter, rand in the till

MoneyBadger lets shoppers pay with Lightning at retailers including Pick n Pay and, since April 2026, hundreds of Engen fuel stations; merchants are paid in rand the next business day ([TechCentral](https://techcentral.co.za/bitcoin-payments-mainstream-south-africa/267462/), [Blink](https://blink.sv/blog/weekly-brief-2026-15)). Ten wallets can pay, six of them Lightning wallets ([Blink](https://blink.sv/blog/weekly-brief-2026-24)). In 2025 it ran at about 1,600 outlets and R1.4 million (about $83,000) a month ([Daba Finance](https://www.dabafinance.com/en/news/moneybadger-crypto-payments-south-africa-bitcoin-retail-adoption)).

**What it shows:** acceptance through existing retail payment networks scales reach quickly. Spending stays small next to it.

### Brazil: local money on a bitcoin layer

BTCPay Server's DePix plugin lets customers pay a merchant with a Pix QR code, settling in DePix, a stablecoin pegged to the Brazilian real on the Liquid network ([BTCPay Server](https://blog.btcpayserver.org/depix-plugin/)). In the first quarter of 2026, DePix made up roughly half of Liquid's 1.16 million transactions ([Liquid](https://blog.liquid.net/liquid-federation-quarterly-update-q1-2026/)).

**What it shows:** the most-used asset on a bitcoin layer, by transaction count, is a local-currency token tied to a national payment system. That supports [Stablecoins, unpacked](03-stablecoins.md): outside dollarizing economies, people want their own currency.

### Boltz: non-custodial, and still gone

Boltz ran atomic swaps between on-chain bitcoin, Lightning, Liquid and, from March 2026, USDT. On August 1, 2026 a bug disabled its swaps into tokens on other blockchains; on August 3 it suspended all swaps "until further notice," citing AI-assisted attacks: "attackers now iterate faster than a team our size can find and patch." Because it never held user funds, "no user funds were ever at risk," and refunds still work, including without Boltz ([Bitcoin News](https://bitcoinnews.com/p/boltz-suspends-bitcoin-services-ai-assisted-attacks)). The founders stepped down; new operators are taking over, with no restart date ([Bitcoin News](https://bitcoinnews.com/p/boltz-new-veteran-bitcoiners-take-over), August 2026). Wallets that depended on it, including Aqua and Bull Bitcoin, had to find replacements ([The Defiant](https://thedefiant.io/news/defi/bitcoin-bridge-boltz-halts-swaps-indefinitely-citing-ai-assisted-attacks)), and Blockstream launched a swap service in closed beta ([Diario Bitcoin](https://www.diariobitcoin.com/blockchain/blockstream-lanza-su-servicio-de-swaps-tras-el-cierre-de-boltz-por-ataques-de-ia/)).

**What it shows:** non-custodial design protects funds, not availability. A wallet with one swap provider has one point of failure.

## The plumbing

### Between layers

| Path | How it works | Who's trusted | Source |
| --- | --- | --- | --- |
| Ark (Arkade) to Lightning | A "solver" pays the invoice, then claims the user's locked funds; 0.30% fee; 335–200,000 sats; beta | The solver for availability only; funds refund after a timeout | [Arkade docs](https://docs.arkadeos.com/contracts/lightning-swaps) |
| Ark (Bark) to and from Lightning | Second's Ark server runs the Lightning node; sending is protected by a hash-locked contract; receiving requires trusting the server "actually deleted the ephemeral key" | The server, partly, when receiving | [Second docs](https://second.tech/docs/learn/payments-lightning) |
| Spark to Lightning | A provider pays; Spark's operators lock the sender's funds until it proves payment | Spark's operators | [Spark docs](https://docs.spark.money/learn/lightning) |
| Cashu to Lightning or on-chain | The mint pays on the wallet's behalf ("melting") | The mint, fully | [Cashu NUT-05](https://github.com/cashubtc/nuts/blob/main/05.md) |
| Liquid to Lightning | Mostly Boltz, offline since August 2026 | — | (above) |

**Lightning is the common bridge.** Ark, Spark, Cashu and Fedimint all pay and receive over Lightning through a server, solver or gateway. Balances don't move directly between systems; everything crosses through Lightning or a swap.

**Choosing between providers:** Kaleidoswap's SSPS, a draft standard for wallets to discover swap providers, covers on-chain, Liquid, Arkade, Bark, Lightning and RGB, but not Spark or Taproot Assets. It's at Draft 2 (September 2026), "Not a finalized standard," and lists no adopters ([SSPS](https://github.com/kaleidoswap/ssps)).

### Inbound liquidity

Lightning wallets need inbound capacity to receive. Three models exist in 2026:

- **Channels from a provider** through the LSPS standards (bLIP-50, 51, 52 and 55, all "Active" ([bLIPs](https://github.com/lightning/blips))). LDK implements all four, with server support in beta ([lightning-liquidity](https://docs.rs/lightning-liquidity)). "Most wallets still rely on a single integrated provider" ([Spark research](https://www.spark.money/research/lightning-lsps-specification-progress), August 2026).
- **One channel resized as needed** (splicing), as Phoenix does.
- **No channels at all:** the Ark server or Spark operator supplies liquidity.

### Addressing

| Standard | What it is | Status |
| --- | --- | --- |
| Lightning Address (LUD-16) | `name@domain`, resolved by a web server at that domain | Widely used; no adoption figures ([LUDs](https://github.com/lnurl/luds)) |
| BIP-353 | Payment instructions in signed DNS records, shown as ₿name@domain | "Complete" as a standard ([BIP-353](https://github.com/bitcoin/bips/blob/master/bip-0353.mediawiki)); supported by Phoenix, Zeus, Cake Wallet, Sparrow and others, per a competitor's comparison ([Spark](https://www.spark.money/tools/bitcoin-bip353-vs-lnurl-payment-address-comparison)) |
| BOLT-12 offers | Reusable Lightning payment requests, no web server needed | Supported by Core Lightning, LDK and Eclair; LND "does not natively support BOLT12 as of mid-2026" ([Spark research](https://www.spark.money/research/lightning-bolt12-adoption-progress)) |
| Phone numbers | `phonenumber@bitcoin.co.ke` | Kenya only (Tando) |

*Several descriptions in this section come from Spark's research pages; Spark builds a competing layer.*

## Getting in and out

- **Peer-to-peer exchanges that work with self-custody are under pressure.** Paxful shut down on November 1, 2025 ([Spark](https://www.spark.money/tools/bitcoin-p2p-exchange-comparison)). Peach stopped co-signing trade releases on September 1, 2026 after a Swiss regulatory review and capped buys at CHF 500 ([CryptoTicker](https://cryptoticker.io/en/peach-bitcoin-escrow-suspended/)). An attacker took 11.59 BTC from 10 Bisq users in an exploit limited to altcoin trades ([Bisq](https://bisq.network/blog/security-incident-post-mortem/), May 2026). Platform fees range from under 0.2% (RoboSats) to 2% for buyers (Peach) ([Spark](https://www.spark.money/tools/bitcoin-p2p-exchange-comparison)).
- **Apps.** Strike costs roughly 1.2% all-in at its base tier; Cash App 2–2.75% on small buys, with no fee or spread on purchases over $2,000 since February 2026 ([Spark](https://www.spark.money/tools/strike-vs-cash-app-bitcoin-comparison)). Cash App's bitcoin features are US-only.
- **ATMs: expensive, and a scam channel.** There were 38,928 crypto ATMs worldwide in March 2026, 78% of them in the US ([Bitcoin.com News, citing Coin ATM Radar](https://news.bitcoin.com/en/crypto-atm-count-falls-to-38928-as-597-machines-exit-the-market-in-q1-2026/)). The median fee to buy bitcoin at one was 16%, by operators' own reports ([Kansas City Fed](https://www.kansascityfed.org/research/payments-system-research-briefings/the-controversial-business-of-cash-to-crypto-bitcoin-atms/), 2023). Americans lost over $388 million to scams using crypto ATMs in 2025, mostly people over 50 ([BleepingComputer, citing the FBI](https://www.bleepingcomputer.com/news/security/fbi-americans-lost-over-388-million-to-scams-using-crypto-atms-in-2025/)). Indiana, Tennessee, Vermont, Minnesota and Hawaii have banned them in whole or in part ([ATM Marketplace](https://www.atmmarketplace.com/articles/where-are-bitcoin-atms-banned/), October 2026).
- **Round-trip cost.** A comparison puts bitcoin and Lightning at 0.5–1.5% for US to Mexico or the Philippines, against 3.5–6% for traditional remittances, and cites the World Bank's average of 6.36% for sending $200 ([Spark](https://www.spark.money/tools/bitcoin-remittance-corridor-comparison)). No independent study adds up buying, sending and cashing out; an ATM purchase alone would cancel the savings.
- **Remittances run on stablecoins.** Bitso says it carried 14.7% of US-to-Mexico remittances in January–August 2026, using stablecoins and paying out pesos ([Rio Times](https://www.riotimesonline.com/mexico-bitso-15-percent-remittances-2026/)).

## The rules

| Where | What applies to conversion services | Status |
| --- | --- | --- |
| Kenya | License from the central bank for payment-facing services (minimum capital KES 10 million for processors, KES 150 million for wallet providers); local incorporation and a resident CEO; sender and recipient information travels with transfers ([CM Advocates](https://cmadvocates.com/blog/the-virtual-asset-service-providers-regulations-2026/)) | Regulations gazetted July 2026; existing operators had until November 4, 2026 |
| Brazil | Central bank authorization; providers must identify the owner of self-custody wallets they send to ([Ledger](https://www.ledger.com/pt-br/licenca-spsav-exchanges-banco-central)); banks can't deal with unauthorized providers from November 6, 2026 | 24 firms authorized and 143 applications pending at the deadline ([Finsiders](https://finsidersbrasil.com.br/?p=376268)); Bitso left Brazil ([Jornal do Comércio](https://www.jornaldocomercio.com/economia/2026/10/1268919-empresas-cripto-se-preparam-para-nova-regulacao-do-banco-central-e-mercado-se-consolida.html)) |
| EU | MiCA authorization for exchanging crypto for money; unauthorized providers had to stop from July 1, 2026 ([FSMA](https://www.fsma.be/en/news/crypto-assets-service-providers-end-transitional-period)) | 394 providers authorized ([CASP Tracker](https://casptracker.eu/what-is-casp/)) |
| South Africa | Licensing by the FSCA; the travel rule covers transfers to self-custody wallets, with no minimum amount within a business relationship ([Moonstone](https://www.moonstone.co.za/fic-tightens-crypto-rules-no-data-no-transfer-standard-emerges/)) | 300 of 512 applicants approved by December 2025 ([Moonstone](https://www.moonstone.co.za/fsca-licenses-most-crypto-provider-applicants-as-enforcement-tightens/)) |
| Nigeria | Proposed: local incorporation, resident CEO, minimum capital up to ₦2 billion ([Nairametrics](https://nairametrics.com/2026/08/22/sec-sets-n30-million-registration-fee-up-to-n2-billion-capital-for-crypto-firms/)) | Proposed, August 2026 |

**What it shows:** the provider at the conversion step becomes a licensed, local business that collects identity data, including about self-custody wallets. That raises the cost of running a last-mile bridge and favors fewer, larger providers.

## Privacy at the edge

- **Personal identifiers as payment keys leak.** About 47.9 million Pix keys have been exposed in incidents since 2020, most of them in one 2025 breach, revealing names and partial bank details ([Jornal de Brasília](https://jornaldebrasilia.com.br/noticias/brasil/quase-48-milhoes-de-chaves-pix-foram-expostas-em-incidentes-desde-2020-diz-banco-central/), citing the central bank). An earlier field study of Pix found the same risk of leaks and scams ([Sacramento](https://www.psacramento.com/pix-in-brazil-a-field-study-for-the-bitcoin-community/)).
- **Lightning addresses expose the payer.** Paying one sends a web request to the recipient's domain, which reveals the payer's IP address and timing ([Spark glossary](https://www.spark.money/glossary/lightning-address)). Phone-number addresses add a real-world identifier on the recipient's side; Blink's Tando announcement says "The privacy trade-off is acknowledged" without explaining it.

## Lessons from elsewhere

How payment interoperability got adopted elsewhere:

- **A coordinator or mandate speeds it up.** India's UPI was interoperable from day one under a central operator; "Most UPI transactions take place across different apps" ([IMF](https://www.imf.org/en/publications/fandd/issues/2025/09/indias-frictionless-payments-maria-peria), 2025). Brazil made Pix mandatory for institutions with 500,000 or more accounts; it became the most-used electronic payment method within about 18 months, at an average cost to businesses of 0.33% against 1.13% for debit cards and 2.34% for credit cards ([Banco Central do Brasil](https://www.bcb.gov.br/content/estabilidadefinanceira/pix/relatorio_de_gestao_pix/relatorio_gestao_pix_2023.pdf)).
- **Or no dominant provider.** Tanzania's mobile money providers connected their networks voluntarily between 2014 and 2016; transfers between networks grew from about 5% to about 28% of person-to-person mobile money ([BFA for CGAP](https://www.findevgateway.org/sites/default/files/publications/files/tanzania_interoperability_post-implementation_review_21_feb_2018_wdisclaimer.pdf), 2018). Kenya, where M-Pesa dominated, connected wallets only in 2018 and merchants in 2022, under central bank pressure ([CGAP](https://www.cgap.org/blog/east-african-interoperability-dispatches-home-of-m-pesa), [The Star](https://www.the-star.co.ke/news/world/2022-04-08-airtel-telkom-users-can-now-use-lipa-na-m-pesa-service)).
- **Open standards still concentrate.** In India, "over 95 percent of UPI transactions are initiated using only three apps" ([IMF](https://www.imf.org/en/publications/fandd/issues/2025/09/indias-frictionless-payments-maria-peria)).
- **One code, many routes.** Singapore's SGQR replaced separate codes from 27 payment schemes with one label ([MAS](https://www.mas.gov.sg/news/media-releases/2018/singapore-introduces-worlds-first-unified-payment-qr-code), 2018), and EMVCo's merchant QR lets one code carry several providers' schemes ([EMVCo](https://www.emvco.com/knowledge-hub/the-what-why-and-how-of-emv-qr-codes/)). That's the closest model to a merchant code that accepts both bitcoin and local payment systems.

**What it suggests:** bitcoin's layers are interoperable by design, but without a coordinator, mandates or zero-cost pricing, adoption depends on providers choosing to connect, and the front ends may concentrate anyway.

## Sizing

| Measure | Figure | Source |
| --- | --- | --- |
| Liquid transactions, Q1 2026 | 1.16 million, about half DePix | [Liquid](https://blog.liquid.net/liquid-federation-quarterly-update-q1-2026/) |
| MoneyBadger, 2025 | about R1.4 million (about $83,000) a month | [Daba Finance](https://www.dabafinance.com/en/news/moneybadger-crypto-payments-south-africa-bitcoin-retail-adoption) |
| Tando, mid-2025 | over 100 transactions a day | [Crypto Briefing](https://cryptobriefing.com/bitcoin-lightning-payments-kenya-tando/) |
| Merchants on BTC Map, October 2026 | 27,330 listed, 15,684 verified in the past year | [BTC Map](https://blog.btcmap.org/posts/2026-10/) |
| Crypto ATMs, March 2026 | 38,928 | [Bitcoin.com News](https://news.bitcoin.com/en/crypto-atm-count-falls-to-38928-as-597-machines-exit-the-market-in-q1-2026/) |

The counted last-mile flows are small and scattered. The largest numbers are reach (addresses, merchants enabled), not use.

## Key assumptions

1. **Recipients mostly want local money.** Supported everywhere observed. Contradicted if Kenyans claim their numbers in large numbers to keep bitcoin.
2. **Reach through existing systems beats building new acceptance.** Supported by MoneyBadger and Tando. Unclear whether reach turns into payments.
3. **Provider choice can be standardized.** Not yet supported: SSPS has no adopters, and most wallets use one provider per function.
4. **Licensing will consolidate providers.** Supported by Brazil's exits and Kenya's capital requirements.

## What could serve this

**Kinds of product**

- **Standards:** Pave, SSPS, Lightning addresses on phone numbers, BIP-353 names.
- **Conversion services** into local money (Tando, Bull Bitcoin, Bringin) or local stablecoins (DePix).
- **Directories** that map phone numbers or handles to payment addresses.
- **Merchant plugins** for local payment systems (BTCPay's DePix plugin).
- **Swap providers** between bitcoin layers and assets, ideally several per wallet.

## Trade-offs for self-custodial, client-side products

- **Lightning addresses already reach some local systems:** a wallet that can pay a Lightning address can pay any Kenyan M-Pesa number today, with no extra integration.
- **Conversion happens at a provider,** so "self-custodial end to end" usually means the user holds their own funds while a licensed provider handles conversion. Atomic swaps narrow that gap for funds, not for availability.
- **Choice of provider is the lock-in and resilience question:** SSPS-style discovery would let a wallet switch when a provider exits, as Boltz did. Pave aims for the same across local payment systems.
- **Inbound liquidity ties wallets to providers:** most Lightning wallets rely on one liquidity provider; Ark and Spark wallets rely on their operator.
- **Design matters at the edge:** showing who receives what, in which currency, at what cost, and through which provider, clearly and before the user pays.

## Risks and open questions

**Risks**

- **Provider exit:** Boltz's suspension and Bitso's exit from Brazil show how quickly a route can disappear.
- **Regulation:** conversion is now licensed in most of the countries studied, with identity checks that reach self-custody wallets.
- **Privacy:** phone numbers and other personal identifiers as payment addresses enable leaks and scams.
- **Scams at the on-ramp:** crypto ATMs are a major scam channel, which drives bans that also affect legitimate users.
- **Fragmentation:** each country has its own system and provider, so coverage grows slowly.

**Open questions**

1. How many payments to M-Pesa numbers via Tando happen, and do recipients claim their addresses (keep bitcoin) or take shillings?
2. Is there any route from Lightning to Korean won, or to Pix keys and Argentine QR codes, beyond prototypes?
3. Who will restart Boltz-style swaps, and will wallets adopt more than one swap provider?
4. Could Pave be built as a thin standard on top of what Tando and DePix already do?
5. What does the round trip actually cost, from buying bitcoin to the recipient's local money, in a few real corridors?

## Research plan: say, do, make

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Test payments | Do | Small real payments through each bridge in the table above | Fees, speed, failure modes, what the recipient sees |
| Round-trip costing | Do | Three corridors (US–Mexico, UK–Kenya, EU–Nigeria) | Total cost from buying to cash-out, against remittance services |
| Provider interviews | Say | 5 last-mile providers | Volumes they'd share, licensing costs, what they need from wallets |
| Recipient interviews | Say | Kenyan M-Pesa users who received via Tando | Whether they claimed their number, and why |

**Outputs:** a tested country map, a round-trip cost table, and an updated thesis.

## Sources

**Countries:** [Alvarez, Argente and Van Patten: Bitcoin as legal tender in El Salvador](https://www.davidargente.com/_files/ugd/b05023_7825615207654784864b4c4cc4ec6550.pdf) · [Blink: 40 million Kenyans now have a bitcoin Lightning address](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address) · [Crypto Briefing on Tando](https://cryptobriefing.com/bitcoin-lightning-payments-kenya-tando/) · [Pave: a protocol for last-mile bitcoin](https://gbks.substack.com/p/pave-protocol-for-last-mile-bitcoin) · [TechCentral on MoneyBadger](https://techcentral.co.za/bitcoin-payments-mainstream-south-africa/267462/) · [Daba Finance on MoneyBadger](https://www.dabafinance.com/en/news/moneybadger-crypto-payments-south-africa-bitcoin-retail-adoption) · [Blink weekly brief, April 2026](https://blink.sv/blog/weekly-brief-2026-15) · [Blink weekly brief, June 2026](https://blink.sv/blog/weekly-brief-2026-24) · [Technext on Tapnob](https://technext24.com/crypto/tapnob-nigeria-crypto-to-naira-gateway/) · [Bitnob docs on Nigerian payouts](https://bitnob.dev/docs/payouts/corridor-specific-behavior/nigeria-payout) · [BTCPay Server: DePix plugin](https://blog.btcpayserver.org/depix-plugin/) · [Liquid quarterly update, Q1 2026](https://blog.liquid.net/liquid-federation-quarterly-update-q1-2026/) · [NostrPIX](https://www.btcplusplus.dev/floripa/hackathon/projects/74350840-a01a-4a79-9cb4-8b756373ecf1) · [Bull Bitcoin on paying in Mexico](https://bullbitcoin.com/blog/how-to-pay-with-bitcoin-at-any-business-in-mexico) · [FinanzWire on Aureo and Amboss](https://www.finanzwire.com/press-release/amboss-and-aureo-connect-the-lightning-network-to-mexicos-banking-system-XezkkOlnWrx) · [Bitcoin Magazine on Pouch](https://bitcoinmagazine.com/business/400-small-businesses-in-the-philippines-are-now-accepting-bitcoin) · [Bitcoin.com News on Coins.ph](https://news.bitcoin.com/coins-ph-adds-bitcoin-and-ethereum-to-national-qr-ph-reaching-700000-philippine-merchants/) · [Bitcoin Magazine on Aurora](https://bitcoinmagazine.com/news/japanese-bitcoin-industry-unveils-aurora) · [Bringin](https://bringin.app/) · [Bitcoin Magazine on Square](https://bitcoinmagazine.com/news/square-crosses-1-million-bitcoin-merchants) · [Cointelegraph on Steak 'n Shake](https://cointelegraph.com/news/steak-n-shake-bitcoin-accumulation-strategic-reserve-btc-payments)

**Plumbing:** [Bitcoin News on Boltz's suspension](https://bitcoinnews.com/p/boltz-suspends-bitcoin-services-ai-assisted-attacks) · [Bitcoin News on Boltz's new operators](https://bitcoinnews.com/p/boltz-new-veteran-bitcoiners-take-over) · [The Defiant on Boltz](https://thedefiant.io/news/defi/bitcoin-bridge-boltz-halts-swaps-indefinitely-citing-ai-assisted-attacks) · [Diario Bitcoin on Blockstream Swaps](https://www.diariobitcoin.com/blockchain/blockstream-lanza-su-servicio-de-swaps-tras-el-cierre-de-boltz-por-ataques-de-ia/) · [Arkade docs: Lightning swaps](https://docs.arkadeos.com/contracts/lightning-swaps) · [Second docs: Lightning payments](https://second.tech/docs/learn/payments-lightning) · [Spark docs: Lightning](https://docs.spark.money/learn/lightning) · [Cashu NUT-05](https://github.com/cashubtc/nuts/blob/main/05.md) · [Kaleidoswap SSPS](https://github.com/kaleidoswap/ssps) · [bLIPs](https://github.com/lightning/blips) · [lightning-liquidity](https://docs.rs/lightning-liquidity) · [Spark research on LSP specifications](https://www.spark.money/research/lightning-lsps-specification-progress) · [LUDs](https://github.com/lnurl/luds) · [BIP-353](https://github.com/bitcoin/bips/blob/master/bip-0353.mediawiki) · [Spark on BIP-353 and LNURL](https://www.spark.money/tools/bitcoin-bip353-vs-lnurl-payment-address-comparison) · [Spark research on BOLT-12 adoption](https://www.spark.money/research/lightning-bolt12-adoption-progress)

**Getting in and out:** [Spark's P2P exchange comparison](https://www.spark.money/tools/bitcoin-p2p-exchange-comparison) · [CryptoTicker on Peach](https://cryptoticker.io/en/peach-bitcoin-escrow-suspended/) · [Bisq post-mortem](https://bisq.network/blog/security-incident-post-mortem/) · [Spark on Strike and Cash App](https://www.spark.money/tools/strike-vs-cash-app-bitcoin-comparison) · [Bitcoin.com News on ATM counts](https://news.bitcoin.com/en/crypto-atm-count-falls-to-38928-as-597-machines-exit-the-market-in-q1-2026/) · [Kansas City Fed on ATM fees](https://www.kansascityfed.org/research/payments-system-research-briefings/the-controversial-business-of-cash-to-crypto-bitcoin-atms/) · [BleepingComputer on ATM scams](https://www.bleepingcomputer.com/news/security/fbi-americans-lost-over-388-million-to-scams-using-crypto-atms-in-2025/) · [ATM Marketplace on bans](https://www.atmmarketplace.com/articles/where-are-bitcoin-atms-banned/) · [Spark's remittance corridor comparison](https://www.spark.money/tools/bitcoin-remittance-corridor-comparison) · [Rio Times on Bitso's remittances](https://www.riotimesonline.com/mexico-bitso-15-percent-remittances-2026/) · [BTC Map, October 2026](https://blog.btcmap.org/posts/2026-10/)

**Rules and privacy:** [CM Advocates on Kenya's regulations](https://cmadvocates.com/blog/the-virtual-asset-service-providers-regulations-2026/) · [Ledger on Brazil's licensing](https://www.ledger.com/pt-br/licenca-spsav-exchanges-banco-central) · [Finsiders on Brazil's applications](https://finsidersbrasil.com.br/?p=376268) · [Jornal do Comércio on Brazil's market](https://www.jornaldocomercio.com/economia/2026/10/1268919-empresas-cripto-se-preparam-para-nova-regulacao-do-banco-central-e-mercado-se-consolida.html) · [FSMA on MiCA's transition](https://www.fsma.be/en/news/crypto-assets-service-providers-end-transitional-period) · [CASP Tracker](https://casptracker.eu/what-is-casp/) · [Moonstone on South Africa's licensing](https://www.moonstone.co.za/fsca-licenses-most-crypto-provider-applicants-as-enforcement-tightens/) · [Moonstone on the travel rule](https://www.moonstone.co.za/fic-tightens-crypto-rules-no-data-no-transfer-standard-emerges/) · [Nairametrics on Nigeria's proposed rules](https://nairametrics.com/2026/08/22/sec-sets-n30-million-registration-fee-up-to-n2-billion-capital-for-crypto-firms/) · [Jornal de Brasília on Pix key leaks](https://jornaldebrasilia.com.br/noticias/brasil/quase-48-milhoes-de-chaves-pix-foram-expostas-em-incidentes-desde-2020-diz-banco-central/) · [Sacramento: Pix in Brazil](https://www.psacramento.com/pix-in-brazil-a-field-study-for-the-bitcoin-community/) · [Spark glossary: Lightning address](https://www.spark.money/glossary/lightning-address)

*Research for this draft was done with AI agents, each claim checked against an opened source; Boltz's suspension and Tando's custody wording were rechecked by hand. Spark's comparison and research pages are cited often here; Spark builds a competing product, so treat them as directional.*
