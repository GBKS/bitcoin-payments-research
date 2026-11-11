# Payments that feel different

*Deep dive, first draft, focused on gifting and payments as expression. Builds on the November 8 quick scan. Last updated November 11, 2026.*

## Thesis

People pay readily, and repeatedly, when a payment carries meaning: a gift, a message, recognition, a game. Ordinary payments are neutral transfers; these payments are social acts. Two things follow from the evidence:

1. **Rituals spread payments socially.** Receiving a meaningful payment makes people more likely to send one, so the behavior travels through groups without marketing.
2. **Expressive payments are already big businesses on other rails,** usually inside closed platforms that take a large cut or lock value to merchants.

**The hypothesis:** a payment experience designed around a ritual or a moment of expression can bring people into bitcoin payments who would never have come for the money itself, and turn recipients into senders.

*Status: working hypothesis. Strong evidence from China, Korea and live streaming; little bitcoin-specific evidence beyond its own community.*

## What we mean

| Form | What it is | Examples |
| --- | --- | --- |
| Gifting rituals | Money given in a culturally defined way, at defined moments | Red envelopes (Lunar New Year), otoshidama (Japanese New Year money for children), wedding and funeral money |
| Social gifting | Sending a gift (often a voucher) to someone in your contacts | KakaoTalk Gift |
| Expressive payments | A payment that is also a visible message | YouTube Super Chats, Twitch Bits, Nostr zaps, podcast "boosts" |
| Playful payments | Chance, games or competition built into paying | WeChat's random group split, play-to-earn games |

Area 11 covers collective payments (pooling toward a goal). This area covers payments where the *act* of paying matters as much as the amount. The two overlap in gifts to idols and fan projects.

## Why existing payments serve them badly

- **Neutral transfers lose the meaning.** A bank transfer can't carry an envelope, a handwritten note or a moment. When otoshidama moved to cashless transfers in Japan, a 61-year-old lamented losing the personal touch of handwritten notes, while a 20-year-old called it "a win-win" because it skips choosing envelopes ([Unseen Japan](https://unseen-japan.com/otoshidama-cashless-japan/), 2020).
- **Platforms take a large cut.** Creators keep 70% of Super Chat revenue, after taxes and iOS or Google Play fees are deducted ([SlashGear](https://www.slashgear.com/1677454/youtube-super-chat-how-much-creators-earn-percentage)).
- **The best experiences live in closed, domestic ecosystems.** WeChat red envelopes and KakaoTalk Gift work inside one app and, in practice, one country.
- **Vouchers lock value to merchants.** Social gifting in Korea is mostly gift certificates for specific brands.
- **Gifting across borders is awkward.** Diaspora families sending red envelopes or otoshidama across countries fall back on bank transfers or gift cards. *[assumption; to research]*

## Case studies

### WeChat red envelopes: a ritual that built a payment system

- WeChat launched red envelopes on January 17, 2014. Group envelopes split a set sum randomly among recipients. During its Spring Festival Gala promotion, 1.2 billion envelopes worth over 500 million yuan went out ([Wikipedia](https://en.wikipedia.org/wiki/WeChat_red_envelope)). Wikipedia dates the promotion to 2014, but the same 500 million yuan was reported for the February 2015 Gala, when users shook their phones 11 billion times ([TechNode](https://technode.com/2015/02/27/wechat-payment-clear-winner-in-tencent-alibaba-digital-lucky-money-war/)). *[to verify: the year and the envelope count, against a primary source]* Because sending or receiving needed a linked bank account, an estimated 100–200 million people added bank details, a figure TechNode calls a rumor that WeChat didn't confirm, and WeChat Pay reportedly more than doubled its market share ([Wikipedia](https://en.wikipedia.org/wiki/WeChat_red_envelope)).
- **Gifts are contagious.** A study of 36.6 million red packets in 174,131 WeChat groups (about 3.45 million users, October 2015 to February 2016) used the random amounts as a natural experiment. Each extra dollar received led recipients to send about 18 cents back to the group within 24 hours, mostly because more people chose to send at all. The "luckiest draw" recipient was much more likely to send the next packet, suggesting a group norm. Gifts also created new connections within groups ([Yuan et al., arXiv](https://arxiv.org/pdf/1906.09698)).

**What it teaches:** the random split turned giving into a game, the group made it visible, and the norm ("the luckiest sends next") kept it going. Payment adoption was a side effect.

### KakaoTalk Gift: social gifting at scale

KakaoTalk Gift was used about 189 million times in 2025 through December 17, about 540,000 gifts a day, across 640,000 gift types from about 8,700 brands. The top gift was a Starbucks voucher. The busiest occasion was Pepero Day (November 11), followed by Valentine's Day and Teachers' Day ([Korea Times](https://www.koreatimes.co.kr/business/companies/20251225/kakaotalk-gifting-service-used-nearly-200-mil-times-this-year)). Kakao's home screen even shows "friends who gifted you around this time" ([Korea Herald via Herald Corp](https://biz.heraldcorp.com/article/10777049)).

**What it teaches:** gifting runs on occasions and contacts. Small, frequent gifts are normal when sending is one tap inside a messaging app.

### Super Chats: expression with a price

Viewers pay $1 to $500 to pin a message in a live chat until someone else pays more, and creators keep 70% after taxes and app store fees ([SlashGear](https://www.slashgear.com/1677454/youtube-super-chat-how-much-creators-earn-percentage)). VTuber income from Super Chats shows stark inequality, increasingly concentrated in two agencies ([arXiv](https://arxiv.org/abs/2503.00825)).

**What it teaches:** people pay to be seen and heard by someone they admire. Visibility and ranking (being on top) are part of the product.

### Japanese otoshidama going cashless

During the COVID-19 period, many in Japan moved otoshidama to Amazon gift cards, PayPay transfers or transit cards, and 51% of survey respondents thought cashless otoshidama was a good idea, with younger people most supportive ([Unseen Japan](https://unseen-japan.com/otoshidama-cashless-japan/), 2020).

**What it teaches:** rituals can move to digital, but the presentation (envelope, note) is part of the gift, and older givers feel its loss.

### Bitcoin's own expressive payments

Nostr zaps passed 142,000 transactions by early March 2023, with about 41 million sats (about $9,250) on the busiest day ([CriptoNoticias](https://criptonoticias.com/tecnologia/ya-enviaron-mas-100000-propinas-bitcoin-nostr)). Value-for-value podcast apps let listeners stream sats or send boosts with messages. *[to verify: current volumes]*

**What it teaches:** the behavior exists in bitcoin's own community and grew fast when it launched, but it's small, and it hasn't spread beyond people who already hold bitcoin.

### Games

Bitcoin Miner, where players earn small amounts of bitcoin through ZEBEDEE, passed 1 million players in March 2023 ([Pocket Gamer](https://www.pocketgamer.biz/bitcoin-miner-surpasses-1-million-players-and-becomes-the-biggest-play-and-earn-game)). Play-to-earn puts sats in front of many people; games where players pay *each other* are untested.

## Other directions (from the quick scan)

- **Mental transaction costs:** cheap payments don't make small payments happen; bundling (tips people choose, credits, budgets) does ([Szabo](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/micropayments.html), [Bitcoin Magazine](https://bitcoinmagazine.com/technical/szabos-micropayments-and-mental-transaction-costs-25-years-later)).
- **Paying without opening an app:** iPhone NFC is open to third parties in the EEA, Australia, Brazil, Canada, Japan, New Zealand, the UK and the US, with Apple's approval, agreement and fees ([MacRumors](https://macrumors.com/guide/apple-nfc-chip-ios-18-1)).
- **Streaming payments** per minute of media, which need a constant connection.

## Sizing

There's no single number, but the scale signals are clear:

| Signal | Scale | Source |
| --- | --- | --- |
| KakaoTalk Gift, 2025 | ~189 million gifts, ~540,000 a day | Korea Times |
| WeChat red envelopes, Spring Festival Gala promotion (2015; Wikipedia says 2014) | 1.2 billion envelopes | Wikipedia, TechNode |
| WeChat red packets studied, 2015–16 | 36.6 million packets in 174,131 groups | Yuan et al. |
| Nostr zaps, first months (2023) | 142,000 transactions | CriptoNoticias |

The gap between the first three rows and the last is the opportunity: the behavior is huge on closed, domestic platforms, and tiny on bitcoin.

## What could serve this

**Kinds of product**

- **Wallet features:** envelopes and themes, payments with messages and stickers, keepsakes.
- **A standalone gifting app or mini-app** around one ritual (red envelopes, otoshidama), which onboards recipients.
- **Messaging integration:** sending a gift inside the chat apps people already use. On iPhone, iMessage apps can send interactive messages *[from memory]*.
- **Streaming and creator tools:** alternatives to Super Chats that creators can add to their streams.
- **Games** with a peer-to-peer economy.

**Trade-offs for self-custodial, client-side products**

- **Recipients without a wallet are the main problem.** Gifts go to people who don't have bitcoin yet. A gift that can be claimed by link solves it, but the funds must either wait with the sender until claimed or be held by someone in between. *[to verify: claim-link options on Ark and Lightning]*
- **The random group split can run on the sender's phone:** split the amount into random shares, create one claimable gift per share.
- **Recipients becoming senders is the growth loop.** The gift contagion study suggests the first gift matters less than whether receiving prompts sending.
- **Gift value in local currency:** givers think in yuan, won or yen, and amounts often carry meaning (auspicious numbers). The amount should be set in local currency at sending.
- **Presentation is the product:** envelopes, notes and moments are design work, not decoration.

## Risks and open questions

**Risks**

- **Novelty:** a beautiful ritual may delight once and not become a habit.
- **Gambling optics:** random splits and games can look like gambling to Apple and regulators.
- **Children:** otoshidama goes to children. Giving minors bitcoin raises questions of consent, custody and app age limits.
- **Authenticity:** rituals belong to cultures; outsiders borrowing them can come across badly.
- **Closed-platform competition:** WeChat and Kakao own their markets; the opening is in diaspora communities and across borders, not head-on.

**Open questions**

1. Did WeChat's red envelopes create lasting payment habits, or a seasonal spike? What carried over to everyday use?
2. In diaspora families, how are red envelopes and otoshidama sent across borders today?
3. Does receiving a bitcoin gift prompt recipients to send one, as with WeChat packets?
4. Which claim mechanism works for recipients without a wallet, without anyone holding funds for long?
5. What makes a digital gift feel personal to an older giver?
6. Do creators and streamers want an alternative to Super Chats, and would their audiences use it?

## Research plan: say, do, make

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 6–8 diaspora families who send red envelopes or otoshidama across borders | How they do it today, what feels lost, who's involved |
| Co-design session | Make | Same families, plus 2–3 designers from those cultures | What a digital envelope should look and feel like |
| Diary study | Do | 10 participants around Lunar New Year 2027 (February 6, 2027, per [Public Holidays](https://publicholidays.com/lunar-new-year/)) | What gifts they send and receive, through which apps, and why |
| Prototype test | Do | 20 senders, their recipients | Claim rates; how many recipients send a gift on |
| Creator interviews | Say | 5 streamers or podcasters who receive tips | What they'd want from an alternative to Super Chats |

**Outputs:** a write-up per method; a "gift journey" map from sender to recipient to new sender.

## Sources

- [Wikipedia: WeChat red envelope](https://en.wikipedia.org/wiki/WeChat_red_envelope)
- [TechNode on WeChat's 2015 Spring Festival Gala campaign](https://technode.com/2015/02/27/wechat-payment-clear-winner-in-tencent-alibaba-digital-lucky-money-war/)
- [Yuan et al.: Gift Contagion in Online Groups: Evidence from Virtual Red Packets](https://arxiv.org/pdf/1906.09698)
- [Korea Times on KakaoTalk Gift in 2025](https://www.koreatimes.co.kr/business/companies/20251225/kakaotalk-gifting-service-used-nearly-200-mil-times-this-year)
- [Herald Corp on KakaoTalk's gifting home screen](https://biz.heraldcorp.com/article/10777049)
- [SlashGear on Super Chat revenue](https://www.slashgear.com/1677454/youtube-super-chat-how-much-creators-earn-percentage)
- [Who Reaps All the Superchats?](https://arxiv.org/abs/2503.00825)
- [Unseen Japan on cashless otoshidama](https://unseen-japan.com/otoshidama-cashless-japan/)
- [CriptoNoticias on Nostr zaps](https://criptonoticias.com/tecnologia/ya-enviaron-mas-100000-propinas-bitcoin-nostr)
- [Pocket Gamer on Bitcoin Miner](https://www.pocketgamer.biz/bitcoin-miner-surpasses-1-million-players-and-becomes-the-biggest-play-and-earn-game)
- [Nick Szabo: Micropayments and Mental Transaction Costs](https://www.fon.hum.uva.nl/rob/Courses/InformationInSpeech/CDROM/Literature/LOTwinterschool2006/szabo.best.vwh.net/micropayments.html)
- [Bitcoin Magazine: Szabo's micropayments 25 years later](https://bitcoinmagazine.com/technical/szabos-micropayments-and-mental-transaction-costs-25-years-later)
- [MacRumors on iPhone NFC access](https://macrumors.com/guide/apple-nfc-chip-ios-18-1)
