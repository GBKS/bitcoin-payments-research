# Money that can't be frozen

*Quick scan. Confidence: medium (well-documented cases, little direct research). Last updated November 8, 2026.*

## The question

Bitcoin's clearest advantage over stablecoins and banks is that nobody can freeze, seize or block it. Most people don't weigh this today; it matters most to people facing capital controls, unstable currencies or being cut off. Who needs censorship resistance *now*, what do they use, and is it a payments need or a savings need?

## What's happening

**Card networks decide what legal businesses can sell.** In July 2025, Steam added a rule against content that may break the standards of payment processors, card networks and banks, and delisted many adult games ([Notebookcheck](https://www.notebookcheck.net/Steam-tightens-adult-content-rules-after-pressure-from-payment-giants.1059462.0.html)). itch.io followed, and DLsite had already lost Visa and Mastercard in 2024 (details in area 11).

**Banks and payment providers cut off activists.** During Nigeria's #EndSARS protests in October 2020, Flutterwave cut off the Feminist Coalition's donation accounts. The group first used a service converting bitcoin into naira, dropped it over the risk of bank freezes, then set up a self-hosted BTCPay Server and raised about 3.14 BTC (about $36,000 at the time) ([CoinDesk](https://www.coindesk.com/nigerian-activists-bitcoin-endsars-police-brutality/)).

**Debanking is political in the US too.** An August 2025 executive order directs regulators to stop "politicized or unlawful debanking," citing firearms dealers, payday lenders and tobacco companies cut off under the Obama-era Operation Choke Point ([Cooley](https://www.cooley.com/news/insight/2025/2025-08-14-executive-order-guarantees-efforts-against-debanking-will-continue)). Which businesses get cut off shifts with politics; that it happens doesn't.

**Stablecoins can be frozen,** and are: over $514 million in 30 days this spring (area 14). Spiral sees possible catalysts in a US crackdown on stablecoin wallets that don't check ID, and in countries restricting dollar stablecoins, as Brazil did for cross-border settlement ([Spiral](https://spiralxyz.substack.com/p/value-stored-now-what)).

**In collapsing currencies, people split the job: stablecoins to spend, bitcoin to save.**

- **Iran:** about $8 billion in crypto activity through Iranian addresses in 2025. People use stablecoins such as Tether for everyday transactions and hold bitcoin as long-term savings, much as Lebanese did when the pound lost 90% of its value in 2019–2021 ([Pulse on CoinDesk](https://www.pulse.bot/crypto/news/irans-rial-collapse-mirrors-lebanons-crisis-driving-citizens-to-bitcoin-dab77748-d289-40ae-b5a0-35bbf0d403d1), February 2026).
- **Bolivia:** with the currency losing more than half its value on the black market and the central bank out of dollars, restaurants and salons accept crypto, mostly USDT (up to an estimated $600,000 a day), while bitcoin is used to protect savings. Crypto transactions rose 530% in the first half of 2025 ([Tiger Brokers news](https://www.itiger.com/news/2546260327)).

**Say versus do:** bitcoiners *say* censorship resistance is bitcoin's killer feature. What people in crises *do* is spend in stablecoins and save in bitcoin. Censorship resistance pulls people toward bitcoin mainly when someone actually freezes or blocks them, as with the Feminist Coalition.

## Who

| Group | What they need | Today's tools |
| --- | --- | --- |
| Legal creators and merchants cut off by card networks | Sales that can't be blocked | Platform-specific workarounds, local bank payments |
| Debanked legal businesses | Accounts and payments that stay open | Cash, smaller banks, high-risk processors |
| Activists and NGOs under hostile governments | Donations that can't be frozen | BTCPay Server, bitcoin donations |
| Savers in collapsing currencies | Savings that hold value and can't be seized | Bitcoin for savings, stablecoins for spending |
| Businesses hit by stablecoin freezes or bans | Dollars or value that can't be frozen | Not yet visible at scale |

## What could serve this

**Kinds of product**

- **Wallets** with strong self-custody, several servers and reliable exit (below).
- **Donation pages** that can't be shut off (self-hosted BTCPay Server, as the Feminist Coalition used).
- **Creator storefronts** with bitcoin checkout for sellers cut off by card networks.
- **Privacy tools,** which matter as much as censorship resistance for at-risk users.
- **Education and setup help** for people who need it urgently, after being cut off.

**Trade-offs for wallets**

- **Self-custody is the core feature here,** more than anywhere else.
- **Ark's weak point:** an Ark server can't take funds, but it can refuse service, and it's run by a company subject to pressure. Unilateral exit to the chain is the fallback, and wallets that support several or custom servers spread the risk across operators. Both matter more in this area than in any other.
- **App stores are a chokepoint too:** Apple and Google can remove apps in a given country, as Apple has in China *[from memory]*.
- **Savings versus payments:** savers want to hold larger amounts long term, which suits cold storage and on-chain wallets more than payment-focused wallets. Donations and creator sales fit payment wallets better.
- **Platforms:** most of the crisis economies are Android-heavy.

## Risks

- **Reputation and Apple:** being seen as a tool for whatever gets cut off attracts scrutiny.
- **Sanctions:** helping people in sanctioned countries can cross legal lines.
- **Safety:** for activists, a payment app's metadata can be dangerous, so privacy matters as much as censorship resistance.

## Open questions for a deep dive

1. What happens *after* someone is cut off? Which tools do they reach for, and how quickly? (Follow real cases.)
2. Would creators cut off by card networks use bitcoin payment pages if buyers could pay easily? What stops buyers today?
3. In crisis economies, does anyone use bitcoin for *payments*, or only for savings?
4. How much does censorship resistance depend on the layer: on-chain, Lightning, Ark with one server, Ark with many?
5. Does privacy matter more than censorship resistance to activists and at-risk users?

## Sources

- [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments)
- [Spiral: Value Stored. Now What?](https://spiralxyz.substack.com/p/value-stored-now-what)
- [Notebookcheck on Steam's adult content rule](https://www.notebookcheck.net/Steam-tightens-adult-content-rules-after-pressure-from-payment-giants.1059462.0.html)
- [CoinDesk on the Feminist Coalition](https://www.coindesk.com/nigerian-activists-bitcoin-endsars-police-brutality/)
- [Cooley on the debanking executive order](https://www.cooley.com/news/insight/2025/2025-08-14-executive-order-guarantees-efforts-against-debanking-will-continue)
- [Pulse on Iran and Lebanon](https://www.pulse.bot/crypto/news/irans-rial-collapse-mirrors-lebanons-crisis-driving-citizens-to-bitcoin-dab77748-d289-40ae-b5a0-35bbf0d403d1)
- [Tiger Brokers news on Bolivian small businesses](https://www.itiger.com/news/2546260327)
