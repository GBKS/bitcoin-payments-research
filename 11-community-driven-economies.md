# Community-driven economies

*Deep dive, first draft. Last updated November 9, 2026.*

## Thesis

There's a large economic space between commerce and charity that existing financial infrastructure barely serves: people pooling, giving and exchanging money to make something happen together, for a community they belong to. Payment systems are very good at paying a merchant. They're much worse at coordinating hundreds of people contributing small amounts toward a shared outcome, often across borders.

These communities already run on improvised tools: personal bank accounts, PayPal Friends & Family, Google Forms and Carrd pages. Trust regularly breaks down, and people outside the home country are often shut out. In these economies money is mostly a coordination mechanism. What people are really after is belonging, recognition and shared achievement.

**The hypothesis:** a self-custodial wallet that coordinates money instead of holding it, and is designed for belonging and expression rather than transactions, can serve these communities better than banks, fintech apps or existing crypto wallets.

*Status: a working hypothesis to test through research. K-pop fandom is the lead case, because these behaviors are unusually developed, visible and culturally accepted there. The same patterns appear in gaming, sports, creator communities, hobby groups and local subcultures.*

## What we mean

**Community-driven economies:** economic activity where the community itself is both the customer and the organizer of value creation. There's no single accepted term. "Fan economy" and "fandom economy" cover the K-pop case. "Participatory economy," "gift economy," "social commerce" and "group buying" each describe one part of it.

The five kinds of transaction overlap, but they have different motivations and mechanics:

| Kind | Shape | Example |
| --- | --- | --- |
| Transactional commerce | I pay you, you give me something | Buying an album in a shop |
| Social commerce | I buy through a social relationship | Buying from a fan you know |
| Collective commerce | We pool money to buy together | K-pop group orders |
| Social patronage | We contribute to support someone or something | Birthday subway ads, gifts, charity in an idol's name |
| Community exchange | We trade within a trusted network | Photocard trading |

The last three are the interesting ones. Existing payments handle the first two reasonably well and the rest badly.

**What these economies revolve around:** belonging and identity, shared goals and collective achievement, supporting someone, recognition within the community, collecting and exchanging, and creating experiences together.

Two examples show the difference. A fan might spend €50 on a group order not because it's the cheapest way to buy an album, but because joining is a social experience. Someone might give €10 toward a subway ad with no personal benefit at all. The reward is collective: *we made this happen.*

## Why existing payments serve them badly

The same problems show up across cases:

- **Money held in personal accounts.** Group funds usually sit in one organizer's bank or PayPal account. That invites embezzlement and opacity, and there's no way to check where the money went.
- **No protection by design.** To avoid fees, organizers ask for payment "without buyer protection." Joiners then have no recourse if an organizer disappears.
- **Borders.** International fans often can't pay into local systems at all: no local bank account, no local card, no local phone number.
- **Card networks as gatekeepers.** Legal creators lose card payments when networks decide their content is too risky. That has happened to Japanese doujin platforms and to itch.io.
- **Built for one-to-one, not many-to-one.** Staged payments (item, then shipping, then shipping again), pledges, rotations and "who has paid" all have to be improvised in spreadsheets and forms.
- **Payments with no meaning attached.** Banks treat every payment as a neutral transfer. These communities care about the message, the recognition and the keepsake.

The workarounds are themselves evidence: Carrd pages, Google Forms, Discord and X threads, and proxy buyers. In design research terms, that's what people *make* when the tools don't fit.

## Case study: K-pop fandom

K-pop is the clearest example. A single fan might take part in fan-app voting, join three group orders a year, trade photocards, chip in for a birthday ad and pay for a fan-run event. That can mean six platforms and several payment methods, so no single dataset captures one person's economic participation.

For scale, the official Circle Chart count was 98.4 million K-pop albums sold in 2024, down from 119.1 million in 2023, with 16.43 million exported. *[from earlier research; verify against the Circle Chart and KPIA originals]* That measures the music business, not the community economy around it. One fan might buy 100 albums through a group order, another one album.

### Group orders (collective commerce)

- **How they work:** international fans pool album and merchandise purchases into one bulk order run by a group order manager. Joiners pay in stages: the item, then international shipping, then domestic shipping. Delivery can take one to six-plus months ([Notes on K-pop](https://notesonkpop.com/the-k-pop-fandom-ecosystem-group-orders-what-they-create/), [Fanlore](https://fanlore.org/wiki/Group_order)).
- **The pain:** managers typically ask for payment without buyer protection, so joiners have no recourse if a manager disappears. Merchandise scams aimed at foreign fans are common. Fraud against foreigners in Korea rose from about 5,300 victims in 2023 to nearly 20,000 in 2025 ([Korea Times](https://www.koreatimes.co.kr/southkorea/law-crime/20260621/fraud-against-foreigners-quadruples-in-2-years-with-k-pop-scams-rising)).
- **The tooling:** Carrd pages, Google Forms, spreadsheets and X threads. Startups such as Paysable and KFriday are building tools for managers. *[to verify]*

### Fan-funded projects (social patronage)

- **What:** subway and outdoor ads, birthday cafés, gifts, charity donations in an idol's name, concert support projects.
- **Scale signal:** K-pop ads on Seoul's subway grew from 76 in 2014 to 1,576 by September 2018, at about $1,300–$4,000 a month per placement ([Korea Herald](https://www.koreaherald.com/article/1803780)).
- **KDOL** (by Hashpurple) is the reference product. It's a crowdfunding app for fan ads, built because most ad funds ran through personal bank accounts and international fans without Korean accounts were shut out. It reports over 400,000 downloads, about 70% international users, and break-even in 2025. It isn't crypto-based ([Wowtale](https://en.wowtale.net/2025/10/09/232389)).
- **Trust failures:** an [SF9 streaming-team moderator embezzling fan donations](https://www.allkpop.com/article/2021/12/moderator-of-sf9s-chart-streaming-team-under-fire-for-embezzling-fans-donations-to-get-into-fansigns-get-their-nails-done-more), and [Song Joong Ki's fan cafe operator apologizing for embezzling funds](https://soompi.com/article/881443wpp/song-joong-ki-fan-cafe-operator-apologizes-embezzling-fan-funds).
- **Regulation:** a [NewJeans fan fundraiser came under legal scrutiny for not being registered](https://www.koreaherald.com/article/10603172), and its organizer was a minor ([allkpop](https://www.allkpop.com/article/2025/10/teen-behind-newjeans-related-fundraising-scandal-sent-to-juvenile-court)).

### Photocard trading (community exchange)

A secondary market with its own conventions, reputation systems and market prices. Worth measuring: listings, completed trades, average values, repeat traders. Starting points: [r/kpopforsale](https://www.reddit.com/r/kpopforsale/) and [r/kpopcollections](https://www.reddit.com/r/kpopcollections/).

### Voting apps and fan platforms

KDOL and similar apps run votes where users watch ads or buy voting credits. One caution: billions of votes don't mean millions of users, because repeated voting is central to the model. The large official platforms are Weverse and Bubble, with paid messaging from idols, community and commerce ([overview](https://respawn.outlookindia.com/pop-culture/pop-culture-guides/weverse-vs-bubble-the-battle-for-k-pop-fans)).

### Fan-run events

Cupsleeve events, birthday cafés, fan exhibitions and group concert activities. They involve real spending that never passes through a conventional retailer.

## Case study: Japan

**Oshikatsu.** Fan activity supporting a favorite idol or character has gone mainstream. An estimated 13.8 million people took part as of January 2025, spending about ¥3.5 trillion a year. One Hakuhodo report found participants devote 37% of their disposable income and 39% of their leisure time to it ([Korea Times](https://www.koreatimes.co.kr/entertainment/k-pop/20250603/oshikatsu-boom-reshapes-japans-youth-economy-and-idol-fandom)). The government sees it as an economic lever ([Asia Times](https://asiatimes.com/2025/04/japan-hopes-oshikatsu-a-fandom-phenomenon-can-boost-its-economy/), [Semafor](https://www.semafor.com/article/04/02/2025/japan-bets-on-fandom)). Spending is highly ritualized and visible, from decorated bags of merchandise to concert travel.

**Creators cut off by card networks.** DLsite, a major platform for games and comics, stopped accepting Visa and Mastercard in April 2024 under pressure over adult content. In October 2025 it launched its own payment option through a Japanese digital bank, which likely isn't available outside Japan ([Automaton](https://automaton-media.com/en/news/japanese-game-and-comic-platform-dlsite-launches-its-own-payment-alternative-following-visa-and-mastercard-suspensions/)). Other Japanese creator platforms lost card support too ([Automaton](https://automaton-media.com/en/news/another-major-japanese-adult-comic-platform-opts-for-diversifying-local-payment-options-amidst-visa-and-mastercard-censorship/)). The same pattern hit itch.io in July 2025: it delisted adult games to keep its payment processors, later restored free ones but kept paid ones blocked, which hurt queer game creators especially ([GamingOnLinux](https://gamingonlinux.com/2025/08/itch-io-to-reindex-free-adult-content-as-they-search-for-new-payment-processors), [Edge Media](https://buffalo.edgemedianetwork.com/story/156870)).

**VTubers and Super Chats.** A study of over a million hours of streams from 1,923 VTubers finds stark income inequality, increasingly dominated by two agencies ([arXiv](https://arxiv.org/abs/2503.00825)). Super Chats are payments as expression: a message, visibly paid for, read out on stream, with the platform taking a large cut.

**A contrast worth noting.** International fans are largely locked out of Japanese live events. But the barrier there is identity, not payment: many shows require a Japanese phone number and residential address, and some check ID at the door ([Unseen Japan](https://unseen-japan.com/japanese-music-foreign-fans-barriers/)). Bitcoin doesn't fix that, and research needs to catch mismatches like this early.

**Apps to study:** Booth (fan-made goods), pixivFANBOX (creator subscriptions) and Skeb (commissions, popular for cross-border requests). *[from memory]*

## Beyond fandom

The same structures appear elsewhere. These are leads, not findings, and none has yet been researched to KDOL's level of specificity.

| Pattern | Examples | What to check |
| --- | --- | --- |
| Collective patronage | Football supporter groups funding banners and stadium displays; charity speedrun marathons with donation messages read live; Twitch communities supporting streamers | Who organizes, how money is collected, how contributors are recognized |
| Collective commerce | Gaming guilds pooling resources; online communities organizing group buys; anime communities funding conventions | Group size, order values, cross-border share |
| Gifting rituals | Lunar New Year red envelopes (WeChat's digital version spread through the ritual itself); Japanese wedding money; Korean wedding and funeral money tracked for years | How presentation and etiquette carry over to digital |
| Rotating savings | Tandas (Mexico), paluwagan (Philippines), arisan (Indonesia), equb (Ethiopia), susu (West Africa), especially in diaspora communities | Trust mechanics, payout rules, attitudes to volatility |
| Scene economies | Berlin club collectives, German club treasuries (Vereinskasse), convention artist alleys, doujin events | Splits, dues, fast small in-person payments |

**China as a warning.** Chinese fan clubs built some of the most intense fan fundraising anywhere, then met a government crackdown: [Weibo banned a BTS fan account for illegal fundraising](https://www.bloomberg.com/news/articles/2021-09-06/china-s-weibo-bans-bts-fan-account-for-illegal-fundraising), and [minors were barred from funding celebrities](https://yicaiglobal.com/news/china-bans-minors-from-economically-support-celebrities-in-efforts-to-tighten-fandom-rules). Background: [Pandaily on China's fan economy](https://pandaily.com/?p=7653).

**The common thread:** money that is social, ritual or expressive. Banks and fintech handle it badly because they treat every payment as a neutral transfer.

## Sizing

Nobody has measured this economy, because it's fragmented across platforms, countries and informal networks. I'd measure three things separately:

1. **Participants:** how many unique people take part.
2. **Economic activity:** how much money changes hands, and how often.
3. **Social coordination:** how many collective transactions, campaigns and exchanges happen.

**What existing data shows, and misses**

| Source | Shows | Misses |
| --- | --- | --- |
| [Circle Chart](https://circlechart.kr/) | Album sales by artist and release | Unique buyers, group-order structure |
| [Hanteo Chart](https://www.hanteochart.com/) | Retail album sales | Informal peer-to-peer trades |
| Customs statistics | Cross-border trade in albums and merchandise | Domestic exchange, individual participants |
| App store rankings | Downloads and ratings | Active users and transactions |
| Fan platforms | Memberships, votes, engagement | Activity outside the platform |
| Social media | Group orders, campaigns, trading communities | Reliable totals |

**A bottom-up method.** Build estimates per segment rather than one global market size. For group orders:

Annual volume = active managers × orders per year × average order value

Purely as an illustration: 10,000 managers × 12 orders × €400 = €48 million a year. *[assumption: every input is illustrative, not data]* Real estimates need to correct for overlap, cancellations, and the difference between retail purchases and money collected from joiners. The same method works for fan projects and secondary markets.

**A dataset worth building.** Track 5–10 major fandoms on: unique participants, transactions per participant, average transaction value, collective versus individual payments, repeat participation, cross-border participation, and money spent on others versus oneself.

The last measure may be the most revealing. How much do people spend on things they personally receive, versus things they create together or give to someone else? That split could show an economic category conventional statistics don't capture at all.

## What could serve this

**Kinds of product**

- **Wallets** with features for groups: staged payments, receipts, payments with messages, keepsakes.
- **Organizer tools:** a group-order manager, a fan project page or a rotation organizer that accepts payment from any Lightning wallet.
- **Platforms** like KDOL, which coordinate campaigns end to end, often holding funds.
- **Gifting apps** built around one ritual, such as red envelopes.
- **Creator tools:** commission flows and tip pages.

Organizer tools are worth noting: organizers are few and influential, and a tool for them doesn't require every joiner to switch wallets.

## Trade-offs for self-custodial, client-side products

Mostly compatible, as long as the app **coordinates money between people and never holds it.**

| Feature | Self-custody | Without your own server | How |
| --- | --- | --- | --- |
| Savings rotation | Fully: no pot exists | Needs shared group state | Each round, everyone pays that round's recipient directly |
| Commissions and payment pages | Fully | Mostly | BOLT-12 offers allow reusable payment requests without a server |
| Staged group-order payments | Fully: each payment goes to the manager | Needs shared group state | Signed receipts per stage; a shared "who has paid" view |
| Payments with messages and stickers | Fully | Mostly | The message travels with the payment |
| Keepsake receipts (wallet passes) | Fully | Partly | Apple Wallet passes must be signed, which normally needs a small backend |
| Fan fund pots | The organizer self-custodies, as with today's personal accounts | Needs shared group state | Works, but transparency is limited (below) |

**Shared state without running a server:**

- **iCloud / CloudKit sharing:** Apple hosts the data and users share records with each other. A good fit for an iOS-only app, but limited to iPhone users.
- **Nostr:** encrypted group events on public relays. Open and cross-platform, but more complex and less reliable.
- **Messaging apps:** state carried in generated links and messages. The simplest, and the weakest at staying in sync.

Reminders to other people need push notifications, which usually need a small relay. Reminders on your own phone can be local.

**Where self-custody genuinely conflicts**

- **Verifiable transparency.** Ark and Lightning payments are private, so contributors can't independently see a pot's total the way KDOL users can. Signed receipts plus a ledger the organizer publishes are the likely compromise. A dedicated on-chain address is publicly auditable, but costs fees and privacy.
- **Spending in fiat.** Seoul Metro and Korean album shops don't take bitcoin, so organizers have to convert, which brings back custody, exchanges and local rules. Pave-style payouts or swaps help with the mechanics only. A conversion partner could handle this part.
- **Joint custody.** Pots controlled by several people (multisig) aren't supported in Bark as far as I know, and on-chain multisig is heavy for small amounts. Design around patterns that avoid pooling. *[to verify: Bark's multi-party and offline-receiving support, with Second]*

## Risks and open questions

**Risks**

- **Fundraising law.** Korea requires larger public fundraisers to be registered, and China has cracked down on fan fundraising. A pot feature has to be designed with this in mind.
- **Minors.** Many fans are teenagers. That affects payments, App Store rules and responsibility.
- **Apple.** App Store review shapes anything involving gambling-like mechanics (voting credits, random draws), adult creators, or in-app purchases.
- **Volatility.** A group order priced in won, or a savings round with a fixed payout, sits badly with a bitcoin balance that moves. People may need prices in local currency, rates locked when an order is created, or swaps.
- **Being an outsider.** These communities have their own norms and reputation systems. A product that arrives from outside, especially one tied to bitcoin's culture, can easily be rejected.

**Open questions**

- Why do organizers use the tools they use today? Fees, habit, what their joiners already have, or something else?
- Is transparency (where the money went) the core pain, or speed, or access from abroad?
- Would fans accept bitcoin as the rail if they never had to think about it? Or does "bitcoin" itself put them off?
- How much of this activity is cross-border, where bitcoin's advantages are biggest?
- Do organizers want a new tool at all, or would they rather keep their own systems and add a better payment step?

## Research plan: say, do, make

Following Liz Sanders' framework: what people **say** (interviews, comments), what they **do** (observed behavior, real transactions), and what they **make** (their own tools and workarounds, plus what they create in generative sessions). Calls for input like Spiral's capture mostly "say." This plan weights "do" and "make."

**First target: K-pop group orders.** A working informal economy run on improvised tools, with a trust problem, cross-border payments at its core, and an audience that fits iOS.

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 5 group order managers, 10 joiners | Motivations, pains, why they use today's tools |
| Tool teardown | Make | Managers' Carrd pages, forms, spreadsheets, terms | What they've already built to cope |
| Money-flow mapping | Make | Managers and joiners, in sessions | Where money, trust and information move, and where they break |
| Following a live order | Do | 2–3 group orders from start to delivery | Real stages, delays, disputes, drop-offs |
| Desk research | Say / do | X, Reddit, Discord communities | Scale, scam patterns, prices, cross-border share |

**Second wave:** fan-funded projects (KDOL users and ad organizers) and one Japanese creator community.

**Field research:** Hongdae and Gangnam stations in Seoul for fan ads. Ikebukuro in Tokyo for oshikatsu goods *[from memory]*. Berlin scenes as a nearby comparison.

**Outputs:** a public write-up of each wave, a money-flow map per niche, and an updated thesis.

*[Open: timing, budget, and whether to recruit through fan communities or a recruiting service.]*

## Sources

**Bitcoin payments context:** [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments), and its [community discussion](https://github.com/spiralxyz/bitcoin-payments/discussions/1).

**K-pop:** [Wowtale on KDOL](https://en.wowtale.net/2025/10/09/232389) · [Korea Herald on subway ads](https://www.koreaherald.com/article/1803780) · [Notes on K-pop on group orders](https://notesonkpop.com/the-k-pop-fandom-ecosystem-group-orders-what-they-create/) · [Fanlore: group order](https://fanlore.org/wiki/Group_order) · [Korea Times on fraud against foreigners](https://www.koreatimes.co.kr/southkorea/law-crime/20260621/fraud-against-foreigners-quadruples-in-2-years-with-k-pop-scams-rising) · [allkpop on fan projects](https://www.allkpop.com/article/2024/12/the-power-of-fan-projects-in-k-pop-supporting-idols-beyond-music) · [Weverse vs. Bubble](https://respawn.outlookindia.com/pop-culture/pop-culture-guides/weverse-vs-bubble-the-battle-for-k-pop-fans) · [Korea Herald on the NewJeans fundraiser](https://www.koreaherald.com/article/10603172)

**Japan:** [Korea Times on oshikatsu](https://www.koreatimes.co.kr/entertainment/k-pop/20250603/oshikatsu-boom-reshapes-japans-youth-economy-and-idol-fandom) · [Asia Times](https://asiatimes.com/2025/04/japan-hopes-oshikatsu-a-fandom-phenomenon-can-boost-its-economy/) · [Semafor](https://www.semafor.com/article/04/02/2025/japan-bets-on-fandom) · [Automaton on DLsite](https://automaton-media.com/en/news/japanese-game-and-comic-platform-dlsite-launches-its-own-payment-alternative-following-visa-and-mastercard-suspensions/) · [Who Reaps All the Superchats?](https://arxiv.org/abs/2503.00825) · [Unseen Japan on ticket barriers](https://unseen-japan.com/japanese-music-foreign-fans-barriers/)

**Card-network exclusion:** [GamingOnLinux on itch.io](https://gamingonlinux.com/2025/08/itch-io-to-reindex-free-adult-content-as-they-search-for-new-payment-processors) · [Edge Media on queer creators](https://buffalo.edgemedianetwork.com/story/156870)

**China:** [Bloomberg on Weibo](https://www.bloomberg.com/news/articles/2021-09-06/china-s-weibo-bans-bts-fan-account-for-illegal-fundraising) · [Yicai on minors](https://yicaiglobal.com/news/china-bans-minors-from-economically-support-celebrities-in-efforts-to-tighten-fandom-rules) · [Pandaily](https://pandaily.com/?p=7653)

*Album sales figures and the sizing framework come from separate earlier research and still need checking against the original sources.*
