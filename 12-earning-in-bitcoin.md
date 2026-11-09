# Earning in bitcoin

*Quick scan. Confidence: low to medium (desk research only). Last updated November 8, 2026.*

## The question

Almost nobody is paid in bitcoin, so spending it means buying it first. Spiral's summary of findings also names earning as the strongest lever. Who actually earns bitcoin today, what do they need, and where does bitcoin beat the alternatives for them?

## What's happening

**The "say" evidence is strong; the "do" evidence is mixed.**

- **Interest is high.** An Oobit survey of 1,004 full-time employees found 43% want some of their pay in digital assets, and bitcoin was the most preferred asset at 46%, far ahead of stablecoins at 11% ([Bitcoin Magazine](https://bitcoinmagazine.com/news/demand-for-crypto-pay-surges-but-payroll-systems-fall-behind-research), April 2026). *Oobit sells crypto payments, so treat this as directional.*
- **But actual crypto pay has moved to stablecoins.** In Pantera's survey of about 1,600 people paid in crypto, stablecoins made up over 90% of 2024 salaries: USDC 63%, USDT 28.6% ([Blockworks](https://blockworks.co/news/stablecoins-salaries-2024-pantera-survey)). That's a reversal from 2022, when bitcoin was the most chosen asset (47%) for Deel's crypto withdrawals, most of which came from Latin America ([Cointelegraph](https://cointelegraph.com/magazine/beyond-the-headlines-the-real-adoption-of-bitcoin-salaries)).
- **Mainstream gig platforms are choosing stablecoins.** DoorDash will let couriers receive earnings in stablecoins via Stripe's Tempo blockchain ([PaymentsJournal via Pulse](https://www.pulse.bot/fintech/news/doordash-to-offer-gig-workers-stablecoin-payouts-63045324-8b01-4649-ae52-06e4eb92a150/), April 2026). Nigerian gig workers prefer stablecoins to the naira for speed, fewer clawbacks and dollar savings; bitcoin comes up only as "jumpy" ([Nairametrics](https://nairametrics.com/2026/02/24/why-nigerian-gig-workers-prefer-stablecoin-payments-to-the-naira/), February 2026).

**The pattern:** where the goal is *dollar income*, stablecoins win. Bitcoin earning is concentrated among people who already want bitcoin.

## Who

| Group | How they earn | What's notable |
| --- | --- | --- |
| Bitcoin industry employees and contractors | Payroll services such as Bitwage and Deel | The largest existing group; the employer often pays in fiat and the service converts |
| Bitcoin-native creators | Nostr zaps, value-for-value podcast apps (Fountain), Stacker News | Small, frequent, social payments; community-driven *[to verify: volumes]* |
| Freelancers paid directly | Lightning invoices, BTCPay Server | Self-custodial and near-instant, but the client has to have bitcoin |
| Micro-task and bounty earners | Task marketplaces such as BitTasker (Nostr-based, Android and web, iOS "coming soon") ([Rootstock docs](https://dev.rootstock.io/dev-tools/wallets/bittasker/)) | Early, small |
| Rewards earners | Sats-back cards such as Fold | "Earning" through spending; custodial *[from memory: details]* |
| Cross-border sellers | Spiral's examples, Trails Coffee and BitTasker | *[to verify: couldn't open either site from here]* |
| Agents | Earning for useful work | See area 13 |

A small, concrete case: a Kenyan worker paid in bitcoin by a European employer through Blink, who pays his internet bill with it because his provider also accepts Blink ([Blink](https://blink.sv/blog/bitcoin-lightning-payments-europe-to-kenya-with-blink-eu), 2024). Earning works best when there's a local loop to spend into.

## Workarounds and players

- **Receiver-side conversion:** the payer pays in fiat and the earner receives bitcoin. Bitwage pioneered this, and processed the first salaries over Lightning in 2021 ([Bitwage](https://bitwage.com/en-us/blog/bitcoin-lightning-network-payroll)). This pattern matters most: *the payer doesn't need bitcoin.*
- **Direct invoices** from Lightning wallets or BTCPay Server: cheap and self-custodial, but technical, and clients rarely pay this way. A comparison by Spark lists the pains: BTCPay's setup, missing fiat conversion, volatility, tax reporting, and low client adoption ([Spark](https://www.spark.money/tools/bitcoin-freelancer-payment-comparison)).
- **Stablecoin payout providers** (Deel, Thunes, Stripe/Tempo) are where mainstream payroll is heading.

## What could serve this

**Kinds of product**

- **Wallets** with good receiving features (below).
- **Invoicing and payment-page tools** for freelancers and creators that work with any Lightning wallet.
- **Payroll and conversion services:** the payer pays in fiat, the earner receives bitcoin. Regulated, usually run by specialist providers.
- **Marketplaces** where work is posted and paid in bitcoin (BitTasker).
- **Local spending loops:** merchants and services that accept what earners receive (the Kenyan internet provider).

**Trade-offs for wallets**

- **Receiving is natural:** usernames and reusable payment requests (BOLT-12), payment pages, invoices, notes and tags, export, and historical fiat values are wallet features, and design matters for them.
- **Payroll needs a conversion provider:** receiving fiat-funded income in bitcoin requires one. A wallet can integrate a provider but not be one.
- **Amounts shape the wallet:** salaries are larger than everyday spending. Payment-focused wallets suit the spending share of income; savings wallets and cold storage suit the rest.
- **Platform:** freelancers in Western markets use both iOS and Android; most stablecoin-heavy earners in Africa and Latin America use Android.

## Risks

- **Tax:** in many countries, receiving and spending bitcoin both create reporting obligations.
- **Volatility:** the main reason earners convert to stablecoins.
- **Regulation:** payroll and conversion are regulated; a wallet partnering with providers inherits some of that.

## Open questions for a deep dive

1. Among people who earn bitcoin today, how much do they keep, and how much do they convert or spend? (Do data, not survey data.)
2. Is receiver-side conversion (pay in fiat, receive bitcoin) the real unlock? Who offers it with self-custodial delivery?
3. Are there earner groups outside bitcoin circles who choose bitcoin over stablecoins, and why?
4. Where do creators earning small Lightning payments (Nostr, podcasts) spend them? Is there a local loop?
5. How does this overlap with community-driven economies (group order managers, fan artists, commissions)?

## Sources

- [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)
- [Bitcoin Magazine on the Oobit survey](https://bitcoinmagazine.com/news/demand-for-crypto-pay-surges-but-payroll-systems-fall-behind-research)
- [Blockworks on Pantera's compensation survey](https://blockworks.co/news/stablecoins-salaries-2024-pantera-survey)
- [Cointelegraph on bitcoin salaries](https://cointelegraph.com/magazine/beyond-the-headlines-the-real-adoption-of-bitcoin-salaries)
- [Pulse on DoorDash stablecoin payouts](https://www.pulse.bot/fintech/news/doordash-to-offer-gig-workers-stablecoin-payouts-63045324-8b01-4649-ae52-06e4eb92a150/)
- [Nairametrics on Nigerian gig workers](https://nairametrics.com/2026/02/24/why-nigerian-gig-workers-prefer-stablecoin-payments-to-the-naira/)
- [Rootstock docs on BitTasker](https://dev.rootstock.io/dev-tools/wallets/bittasker/)
- [Blink on payments from Europe to Kenya](https://blink.sv/blog/bitcoin-lightning-payments-europe-to-kenya-with-blink-eu)
- [Bitwage on Lightning payroll](https://bitwage.com/en-us/blog/bitcoin-lightning-network-payroll)
- [Spark's freelancer payment comparison](https://www.spark.money/tools/bitcoin-freelancer-payment-comparison)
