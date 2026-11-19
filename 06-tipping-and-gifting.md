# What happened to bitcoin tipping and gifting

*Foundation document, first draft. The record of bitcoin (and some other crypto) tipping and gifting products since 2013: how much they were used and how they ended. Desk research only. Last updated November 19, 2026.*

## Why this page

Tips and gifts come up again and again as the natural first use of bitcoin payments: small amounts, social, no merchant needed. They have also been tried many times. Before treating gifting or tipping as an opening ([Payments that feel different](16-payments-that-feel-different.md), [Brand and culture as demand](17-brand-and-culture-as-demand.md)), it's worth knowing what happened to the products that tried.

## The short version

- **No bitcoin tipping or gifting product became a lasting habit at scale.** The pattern repeats: a launch spike, decay to a few hundred enthusiasts, then a quiet end (a switched-off feature, a node that goes dark) or a retreat to licensed countries.
- **Custody ended more products than lack of demand.** Whoever holds the money meets regulators or loses it: dogetipbot, Tippin.me, Coinme, ZBD, Brave, and the LNbits exploit in November 2026.
- **Running costs exceed the value moved.** Founders cite servers, support, bugs and node complexity. No product published revenue that covered its costs.
- **Many gifts are never claimed.** One gifting tool saw a third to two-thirds of its gifts withdrawn; brokers and wallets refund unclaimed gifts after two weeks; one voucher company booked $8.37 million of unredeemed vouchers as income.
- **Tips go to strangers, concentrate and stay tiny.** On Nostr, the top 1% of recipients get most of the value and the median recipient got about 100 sats over three months on the relays sampled.
- **The most committed bitcoin tipping community is moving to dollars.** In 2026 streaming sats in Podcasting 2.0 collapsed, the Podcast Index's Lightning node is closing, and the show's hosts demonstrated boosts paid in USDC.
- **Where it worked, something else carried it:** both sides already in one app (WeChat, Binance, YouTube), a live moment with visible thanks (Super Chats, podcast boosts read on air), or retail distribution (bitcoin gift cards sold in shops and on TikTok Shop).

## Tipping

| Product | Dates | Best usage number found | How it ended or stands |
| --- | --- | --- | --- |
| bitcointip (Reddit bot) | 2013–about 2014 | No totals found ([The Next Web](https://thenextweb.com/news/you-can-now-tip-bitcoin-to-other-users-across-reddit-using-a-cool-new-hack)) | Faded *[from memory; to verify]* |
| ChangeTip | 2014–2016 | About 100,000 users and 350,000+ tips ([Coinspeaker](https://www.coinspeaker.com/bitcoin-micropayments-service-changetip-shutting/)), about 3.5 tips per user *[our arithmetic]* | Team hired by Airbnb; service shut down, citing server, support and site costs |
| dogetipbot (Dogecoin) | 2014–2017 | $150,000 in tips across 56,000 Reddit users, per the founder in 2014 ([Gizmodo](https://gizmodo.com/reddit-users-lose-real-money-after-meme-currency-bot-di-1795125165)) | Company bankrupt; the founder cashed out users' coins and set balances to zero |
| TipJar (Ether, Reddit) | to 2019 | None published | Closed for "very little activity" ([The Block](https://www.theblock.co/news/markets/2019-10-07-crypto-micropayment-service-tipjar-shutting-down-citing-low-usage-42281)) |
| Tippin.me | 2018–2023 | About 14,100 users and 16,500 tips in its first three months, with a spike after one tweet from Jack Dorsey ([Bitcoin Magazine](https://bitcoinmagazine.com/technical/tippinme-takes-lightning-speed-more-14000-new-users)) | Node went offline with no announcement, holding about 9.2 BTC ([No Bullshit Bitcoin](https://nobsbitcoin.com/tippin-me-potential-rug-pull)) |
| LNTXBOT (Telegram) | 2019–2023 | None published | Shut down by its developer, citing "many bugs" and lack of time ([CriptoNoticias](https://www.criptonoticias.com/comunidad/adios-lntxbot-apagan-bot-telegram-enviar-bitcoin)) |
| Twitter Tips with Strike | 2021–about 2022 | About $8,500 in payments worldwide in just over a year, per a BSV-leaning outlet that names no source; we found no primary source ([CoinGeek](https://coingeek.com/twitter-tips-on-lightning-network-fizzles-out-after-1-year-due-to-low-demand/)) | Faded without a formal notice *[to verify]*; bitcoin tips relaunched on X through third parties in August 2025 ([BitcoinNews](https://bitcoinnews.com/p/bitcoin-tips-x-bitbit-spark)) |
| Brave Rewards (BAT, for comparison) | 2018– | 1 million verified creators; 26 million BAT paid to them, cumulative ([Brave](https://brave.com/25m-mau/)) | Running, but cut back: a regulated custodian became mandatory in 2023, citing FinCEN and OFAC ([Brave](https://brave.com/blog/rewards-changes/)). Tips are funded by ad revenue, not users' own money |
| ZBD | 2019– | None published | Left about 90 countries in March 2025 without giving a reason ([ZBD](https://intercom.help/zbd/en/articles/10752774-we-are-discontinuing-zbd-in-certain-regions)); now in 47 countries with an EU license ([The Paypers](https://thepaypers.com/cryptocurrencies/zbd-secures-approval-for-mica-licence-from-dutch-regulator--1271581)) |
| Podcasting 2.0 (value for value) | 2020– | See below | Moving to dollars in 2026 |
| Nostr zaps | 2023– | See below | About tenfold decline on the same relays, 2023 to 2026 |
| Stacker News | 2021– | About 500 active posters a month; 2.7 to 5.0 million sats a month earned from zaps ([September 2026 recap](https://stacker.news/items/1592058), [February 2026](https://stacker.news/items/1451998)) | Small and steady. In September 2026, users spent more on paid ranking (7.5 million sats) than they earned from zaps |

### Podcasting 2.0: from sats to dollars

Value for value let podcast listeners stream sats per minute or send "boosts" with messages, over Lightning. It was the longest-running bitcoin tipping experiment with public data.

- **Usage fell through 2026.** Payments routed through the Podcast Index fell from about 1,300–1,500 a day in early June to about 400 by August, and daily senders from 54–72 to about 20, before the data stopped updating on August 13 ([Podcast Index chart data](https://stats.podcastindex.org/chart-data.json)). *[to verify: read once by a research agent; the endpoint blocks automated checks, and it may cover only payments routed through the Index]*
- **The show itself called it.** The July 17, 2026 episode of Podcasting 2.0 has a segment titled "Streaming sats collapse" ([Podcasting 2.0 feed](https://feeds.podcastindex.org/pc20.xml)); a co-host described streaming sats as "down to pretty well zero" *[to verify: quoted in search results; episode 265 or 266]*. A newsletter reported that the hosts are closing the Podcast Index's Lightning node, under the line "Forget streaming payments. It's over" ([Signal #27](https://buttondown.com/signal-podosphere/archive/signal-27-youtube-overtook-spotify-for-podcast/)). One app developer reportedly declined to build payment splitting because it is "in the money transmitter area" *[to verify]*.
- **The replacement uses dollars.** On November 13, 2026 the hosts demonstrated boosts paid in USDC through the same tag in podcast feeds, "with no server in the middle" ([Podcasting 2.0 feed](https://feeds.podcastindex.org/pc20.xml)); Podnews reported that it "uses dollars, not Bitcoin" ([Podnews](https://podnews.net/update/apple-tv-apple-podcasts)).

**What it teaches:** a committed community, an open standard and years of effort produced a durable habit among a small core (boosts read out on air), but not growth. When the infrastructure cost and legal risk landed on volunteers, they moved to the unit that didn't need a node.

### Nostr zaps: a spike and a long tail

- **Launch:** 142,000 zaps from 8,000+ senders in the first month, with 41 million sats on the busiest day ([CriptoNoticias](https://criptonoticias.com/tecnologia/ya-enviaron-mas-100000-propinas-bitcoin-nostr)); 1 million zaps by June 2023 ([No Bullshit Bitcoin](https://www.nobsbitcoin.com/nostr-protocol-1-million-zaps/)).
- **Same five relays, three years apart** (about 3% of all zaps; one analyst's sample) ([daniella.io](https://daniella.io/nostr-retention-structural-diagnosis/)):

| | February–April 2023 | March–May 2026 |
| --- | --- | --- |
| Zaps | 94,901 | 9,934 |
| Sats | 35.1 million | 2.9 million |
| Share of value to the top 1% of recipients | 72.7% | 60.7% |
| Median received per recipient | 117 sats | 100 sats |

- **Today:** a live daily report showed about 1,200 zaps from 322 senders in 24 hours on November 19, 2026, with about a third of the sats from a single game bot ([NostrZap](https://www.nostrzap.com/dailyreport)).
- **Platform rules:** Apple required Damus to remove zaps on posts in 2023, under its in-app purchase rules ([TechCrunch](https://techcrunch.com/2023/06/26/decentralized-social-networking-app-damus-to-be-removed-from-app-store-will-appeal-decision/)).

## Gifting

| Product | Dates | Best usage number found | How it ended or stands |
| --- | --- | --- | --- |
| Lightning Gifts (original) | 2019 | None found ([code](https://github.com/mikelseverson/react-lightning-gifts)) | Gone. The domain now runs a fork of Lightsats, whose own counter shows 62,271 sats sent in total ([stats](https://lightning.gifts/api/stats)) |
| Lightsats | 2022–2026 | November 2022: 279 tips sent, 95 withdrawn, about 34% ([Stacker News](https://stacker.news/items/94367)); best month: 66% from seen to withdrawn ([BOLT.FUN](https://bolt.fun/story/monthly-review-from-lightsats--609/)) | Gift creation switched off in February 2026, with no announcement found ([commit](https://github.com/lightsats/lightsats/commit/84005714dd148e5c1634129109c88d83c610fc46)) |
| LNbits vouchers | ongoing | None published | Printable claim codes; the giver's server holds the funds until claimed ([docs](https://docs.lnbits.com/extensions/withdraw/)). After an exploit in November 2026, operators were told to shut down ([The Hacker News](https://thehackernews.com/2026/11/lnbits-urges-all-operators-to-shut-down.html)) |
| Bitcoin Laisee (Hong Kong) | 2021 | None published | Lunar New Year red envelopes made from LNbits codes ([Bitcoin Association of Hong Kong](https://www.bitcoin.org.hk/laisee/)) |
| Azteco vouchers | 2019– | More than 1 million buyers, the founder's estimate ([Bitcoin Magazine](https://bitcoinmagazine.com/business/azteco-is-helping-millions-buy-bitcoin-without-sharing-their-identity)) | Running *[to verify]*; mainly a cash-to-bitcoin on-ramp |
| Coinme vouchers (Coinstar kiosks) | to 2023 | $8.37 million of unredeemed vouchers booked as income, according to Washington regulators; Coinme says all vouchers remain redeemable ([Decrypt](https://decrypt.co/350905/coinme-ordered-to-return-over-8m-to-customers-in-washington-state-crackdown)) | Discontinued; regulatory action |
| Fold bitcoin gift card | 2025– | About $1.2 million gift card revenue in Q3 2026, up from about $0.2 million a year earlier ([Yahoo Finance](https://finance.yahoo.com/markets/crypto/articles/fold-holdings-inc-fld-q3-050706987.html)) | **Growing**, sold at Kroger, through Blackhawk and on TikTok Shop, which became its "largest gift card and customer acquisition channel" ([Fold Q3 release](https://www.stocktitan.net/news/FLD/fold-holdings-inc-nasdaq-fld-announces-third-quarter-2026-4qa2tor9qubg.html)). Redemption needs an identity-checked account; redemption rate not published |
| Cash App bitcoin gifts | 2021– | None published | Still offered in December 2024 ([Decrypt](https://decrypt.co/294580/cash-app-has-dropped-its-zero-fee-bitcoin-cashtag-transfers)); the recipient can take dollars instead ([TechCrunch](https://techcrunch.com/2021/12/14/cash-app-now-lets-users-gift-stock-and-bitcoin-using-their-usd-balance-or-a-debit-card/)) |
| Robinhood crypto gifts; Coinbase Wallet send-by-link | 2021; 2023 | None published | Unclaimed gifts refunded after 14 days and 2 weeks ([Fortune](https://fortune.com/2021/12/16/robinhood-send-crypto-gift-bitcoin-ethereum-dogecoin-litecoin/), [The Block](https://www.theblock.co/post/266175/coinbase-rolls-out-money-transfers-via-links-sent-on-whatsapp-tiktok-and-instagram)); current status *[to verify]* |
| Bakkt app; Mudrex "Gift a Crypto" | 2021–2023; to 2026 | None published | Cut as not core to the business ([Decrypt](https://decrypt.co/121208/bakkt-backs-out-of-consumer-business-to-focus-on-b2b-offering), [Mudrex](https://mudrex.com/blog/gift-a-crypto-feature-discontinued-on-mudrex/)) |
| Binance gift cards and red packets | 2021– | Gift cards sent rose 740% in December 2021 against the July–November average, and 70% of redeemers were new users ([Forkast](https://forkast.news/crypto-e-red-packets-lunar-new-year/)). Red packet volume has never been published | Running, mostly as promotions inside the exchange |
| Casascius coins (physical) | 2011–2013 | None published | Stopped after FinCEN treated the maker as a money transmitter ([Bitcoin Magazine](https://bitcoinmagazine.com/business/the-history-and-future-of-physical-bitcoin)) |

A wallet spokesperson in 2022, on crypto red packets: they "aren't really a big thing outside those promotion campaigns" ([Forkast](https://forkast.news/crypto-e-red-packets-lunar-new-year/)).

## Say versus do

- **What founders say:** costs, bugs, lack of time, "low activity," or nothing at all. Post-mortems with numbers are rare; several products ended by switching a feature off.
- **What the data shows:** every launch spiked (a celebrity tweet, a new protocol, a holiday) and decayed within months. The data that survives is mostly from enthusiasts publishing their own stats.
- **Red packets look big and aren't measured.** Exchanges promote them heavily, but none publishes volume, and the activity is driven by campaigns the exchange pays for.

## What the record suggests

1. **Custody is the main cause of death.** Holding users' balances brought money-transmission rules (Casascius, Brave, ZBD, Podcasting 2.0's developers) and loss (dogetipbot, Tippin.me, LNbits).
2. **Infrastructure costs more than tips bring in.** Nodes, support and bug fixes fall on small teams or volunteers.
3. **Spikes are not demand.** Treat launch numbers as noise until they hold for three months or more *[our suggestion]*.
4. **Unclaimed gifts are the norm.** Between a third and two-thirds of link gifts were withdrawn in the one tool that published it. Everyone else built automatic refunds.
5. **Recipients without a wallet are the bottleneck.** Every product that worked had both sides in the same app already, or onboarded recipients into its own account (Fold).
6. **Tips to strangers concentrate.** A few recipients get most of the value, and most creators receive amounts too small to matter.
7. **Units drift to dollars,** even in bitcoin's own communities, when someone has to run the infrastructure (Podcasting 2.0, 2026).
8. **Distribution beats mechanism.** The one growing product (Fold's gift card) grew through shops and a social commerce channel, not through a better claim flow.

## What could serve this

Kinds of product, compared:

| Kind | Example | Who holds unclaimed money | Recipient needs | Record |
| --- | --- | --- | --- | --- |
| Custodial tipping service | ChangeTip, Tippin.me | The service | An account with the service | Closed, often with losses |
| Platform-native tips | Super Chats, Twitter Tips, Brave | The platform or a partner | Nothing new (fiat), or a partner account (crypto) | Works in fiat with live moments; crypto versions faded |
| Claim link from a hosted service | Lightsats, Coinbase Wallet links | The service, until claimed or refunded | Any wallet, or a new one | Small; refunds needed |
| Self-hosted vouchers | LNbits codes, Bitcoin Laisee | The giver's server | Any Lightning wallet | Small; server security risk |
| Gifts inside one app | Cash App, Binance red packets | The app | The same app | Used, mainly through promotions; volumes unpublished |
| Retail gift card | Fold, Azteco | The issuer | An account with the issuer | Growing, as an on-ramp |
| Self-custodial claimable gift | *Not found in this research* | Ideally nobody, or only briefly | Any compatible wallet | Untested *[to verify: what Ark and Lightning allow]* |

The last row is the one no product has shown working: a gift that a recipient without a wallet can claim, where no one holds the funds for long.

## Open questions

1. Is there a way to make claimable gifts without anyone holding the funds for long, on Lightning, Ark or other layers?
2. Did any product publish what share of gift recipients went on to send a gift themselves?
3. What were Twitter Tips' real volumes, and why did they end?
4. What are the redemption rates for retail bitcoin gift cards?
5. Do tips and gifts among people who know each other (rather than to creators and strangers) behave differently?

## Sources

All linked inline. Collected with the help of AI research agents; each link was opened in the course of the research, and the weakest claims were checked a second time, which corrected three figures. Claims still marked *[to verify]* could not be confirmed from a primary source.
