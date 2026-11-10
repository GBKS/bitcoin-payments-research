# Agentic payments

*Deep dive, first draft. Builds on the November 8 quick scan. Desk research only. Last updated November 10, 2026.*

## Thesis

AI agents need small, programmable payments, which Lightning was built for. Yet the first agent payment tools settle mostly in stablecoins, and the evidence below shows a market much smaller than its forecasts:

- **What's real today is machines paying for APIs, in fractions of a dollar.** Agent payments average about $0.48, 76% are below the card networks' $0.30 fee floor, and 98.6% settle in USDC.
- **Measured volume is tiny.** Coinbase's x402, the most used protocol, has moved about $15–19 million in its lifetime once wash and test traffic is removed. Forecasts speak of hundreds of billions to trillions by 2030.
- **People act on AI recommendations but don't let AI pay.** Majorities refuse unapproved agent spending, and OpenAI moved checkout out of ChatGPT's main chat and back to merchants' own apps and sites.
- **Self-custody removes the safety net.** Card and payment-law protections depend on an intermediary. With a self-custodial agent wallet, the only limits are technical ones.

**The hypothesis:** for bitcoin payments, the near-term opening isn't consumers handing agents a budget. It's two narrower things: **people paying per use for AI tools** with small Lightning payments, and **control** for those who fund agents: budgets, approvals, records and an off switch that feel trustworthy. Consumer delegation may come later, and when it does, how control is shown may matter as much as the payment rail.

*Status: a working hypothesis from desk research. Almost every usage figure in this area comes from companies or trade press; independent measurement is the main gap.*

## What we mean

**Agentic payments:** payments initiated by software acting for a person or business, without a human approving each one.

| Kind | Who pays whom | Typical size | Example |
| --- | --- | --- | --- |
| Pay per request | An agent pays an API or service | Fractions of a dollar | x402, L402, Stripe's Machine Payments Protocol |
| Agent shopping | An agent buys goods for a consumer | Tens to hundreds of dollars | Visa Intelligent Commerce, Mastercard Agent Pay, Google's AP2 |
| People paying for AI per use | A person pays per prompt or tool | Cents | PayPerQ |
| Agents earning | An agent sells work or data | Varies | Paid tools, data vending machines |
| Business purchasing | A procurement agent buys within a budget | Large | Corporate cards with agent controls |

**Protocols named here:** x402 (Coinbase's, using the web's "402 Payment Required" status, mostly with USDC); L402 (Lightning Labs', the same idea over Lightning); MPP (Stripe's Machine Payments Protocol, launched with its Tempo blockchain); AP2 (Google's Agent Payments Protocol, which records what a user authorized).

## What people say, and what they do

**Say:**

- In Forrester's April 2026 survey of online adults in the US, UK and Canada, three-quarters were uncomfortable letting an agent buy and pay on its own, **even when they could set spending limits and rules in advance**. A minority would accept it for routine, low-cost purchases under strict thresholds ([Let's Data Science on Forrester](https://letsdatascience.com/news/consumers-reject-delegating-payments-to-ai-agents-447f7acd), June 2026).
- In a MACH Alliance survey of more than 1,000 UK consumers, only 9% were comfortable with AI completing a payment for them. On average, they'd let AI spend about £149 per purchase ([IT Brief](https://itbrief.co.uk/story/uk-shoppers-cap-ai-spending-at-gbp-150-per-purchase), September 2026).
- In a Visa and Morning Consult survey of 2,000 US consumers, 38% were comfortable with AI completing a purchase autonomously, and 60% wouldn't let an agent spend any amount without approval ([The Paypers](https://thepaypers.com/payments/news/visa-research-maps-consumer-and-business-readiness-for-agentic-commerce), April 2026).
- In Riskified's survey of 2,000 US and UK consumers, 55% weren't comfortable with agents buying for them in early 2026, down from about 70% at least somewhat comfortable in late 2025. Half said the AI platform should be responsible for unauthorized purchases ([Digital Transactions](https://www.digitaltransactions.net/many-consumers-say-no-thanks-to-agent-based-payments/), April 2026).
- Across 12,005 consumers in six markets, Checkout.com found people would let an agent spend about £177 per purchase without further approval, with spending limits, instant revocation and easy cancellation as key conditions ([Retail Insider](https://retail-insider.com/retail-insider/2026/06/checkout-com-report-finds-consumer-interest-in-ai-shopping-outpacing-trust-and-merchant-readiness/), June 2026).

*All of these except Forrester's were commissioned by payments or commerce companies; treat them as directional.*

**Do:**

- **Shoppers use AI to research, then buy themselves.** Adobe counts clicks from AI services to US retail sites, not agent purchases. That traffic was up 71% year over year in September 2026 and converted 90% better than other traffic ([Small Business Trends](https://smallbiztrends.com/ai-driven-retail-traffic-surges-71-converts-90-better/), November 2026).
- **In-chat checkout didn't take off.** ChatGPT's Instant Checkout launched in October 2025 with Etsy and Walmart; in March 2026 OpenAI moved purchases to merchants' own apps and checkouts, saying it was evolving "to better meet merchants and users where they are" ([Shopifreaks](https://www.shopifreaks.com/openai-scales-back-its-integrated-commerce-plans/), [American Banker](https://www.americanbanker.com/payments/news/openai-moves-ai-checkout-to-third-parties)).
- **Developers pay for APIs through agents,** which is where real usage is (below).

**Say versus do:** consumers *say* they won't delegate payments, and their behavior matches: they act on AI's suggestions and keep the paying to themselves. Builders *say* an agent economy is arriving; measured activity is a small fraction of the forecasts.

## Why existing payments serve agents badly

- **Card fees don't fit micropayments.** 76% of agent payments fall below the $0.30 fixed fee card networks charge ([Bitcoin.com News on Keyrock's report](https://news.bitcoin.com/keyrock-report-76-of-ai-agent-transactions-fall-below-visas-0-30-fee-floor/), May 2026).
- **Cards assume a human.** Card networks are adding agent identities: Visa's Trusted Agent Protocol, built with Cloudflare, lets agents present signed purchase intent ([Visa](https://usa.visa.com/about-visa/newsroom/press-releases.releaseId.21716.html), October 2025), and Mastercard requires agents to be "registered and verified" ([Mastercard](https://newsroom.mastercard.com/news/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai), April 2025). Most of this is still in pilots.
- **Liability is unsettled.** US consumer protection asks whether a payment was "unauthorized"; a law firm frames the question as whether an agent buying 260 chicken nuggets means the card was stolen ([Dickinson Bradshaw](https://www.dickinsonbradshaw.com/blogs-articles/2026/01/20/new-reg-e-liability-the-ai-bought-that-not-me), January 2026). In the EU, "It remains unclear who bears liability in the event that an AI agent exceeds the scope of its initial mandate" ([Ashurst](https://www.ashurstperkinscoie.com/en/insights/ai-powered-payment-agents-the-next-payments-revolution), November 2025). The UK's FCA is considering whether regulation needs to change ([FCA](https://www.fca.org.uk/publication/regulatory-priorities/payments-report.pdf), March 2026).

## Case studies

### x402: the most used protocol, and how much of it is real

- **Raw versus adjusted.** Of about 178 million x402 transactions and $135.7 million in raw volume, about $15 million remained once wash, test and internal activity was removed, by Visa and Artemis's count as of April 2026; about 5,300 sellers had ever been paid. The filter's thresholds aren't published ([Daniel McGlynn](https://www.danielmcglynn.com/the-x402-counter-has-shown-the-same-four-numbers-since-march/), September 2026).
- **Concentrated and gamed.** On one dataset, "gamed" transactions averaged 64% of all x402 transactions from November 2025 to February 2026 ([Four Pillars, citing Artemis](https://research.4pillars.io/en/research/x402-on-polygon-real-or-gamed)).
- **Falling, then smaller and steadier.** About 99% of x402 payments are in USDC ([Spiral report](https://github.com/spiralxyz/bitcoin-payments)). One analysis counts more than 50 million cumulative x402 transactions, but daily volume fell 92%, from a peak of about 731,000 in December 2025 to about 57,000 ([Agentic Terminal](https://agenticterminal.substack.com/p/the-agentic-settlement-wars)). Adjusted monthly volume fell 77% from November 2025 to $1.19 million in May 2026, while transactions rebounded, at an average of $0.52 each ([CryptoSlate, citing Artemis](https://cryptoslate.com/?p=538356)).
- **Institutional backing anyway.** The x402 Foundation launched under the Linux Foundation in April 2026, with members including AWS, American Express, Cloudflare, Coinbase, Google, Mastercard, Shopify, Stripe and Visa ([Coinbase docs](https://docs.cdp.coinbase.com/x402/support/x402-foundation)).

**What it shows:** a standard with heavyweight support and real but small usage, inflated early by speculation. The payments are for API calls and data, not shopping.

### Card networks and big tech: pilots and walk-backs

- **The big platforms are choosing other rails.** Google's AP2 supports stablecoins through x402, Stripe's Machine Payments Protocol charges agents per API call, and Meta's Muse launched with PayPal and Shop Pay, not bitcoin ([Spiral report](https://github.com/spiralxyz/bitcoin-payments)).
- **Stripe's MPP and Tempo** went live on March 18, 2026, with over 100 services listed; Lightspark extended MPP to Lightning ([The Block](https://www.theblock.co/news/ecosystems/2026-03-18-tempo-mainnet-goes-live-with-machine-payments-protocol-for-agents-394131)). In its first 33 days, MPP carried about $25,000 across about 115,000 transactions, by Artemis's count ([Forkast](https://forkast.news/visa-artemis-the-0-14-reality-of-agent-commerce/), July 2026). *[Forkast's article is AI-written; treat as secondary]*
- **Visa and Mastercard** remain mostly in pilots; a fraud-prevention company counted "hundreds of completed agent-initiated transactions globally" as of September 2026 ([C9 Group](https://c9group.dev/en/articles/agentic-payments-visa-mastercard-stripe-ai-agents)).
- **Forecasts:** Morgan Stanley expects agents to drive up to $385 billion of US online sales by 2030 ([Digital Commerce 360](https://www.digitalcommerce360.com/2025/12/09/morgan-stanley-ai-agentic-shoppers-385-billion-online-sales/amp/), December 2025).

**What it shows:** the largest payment companies are positioning, not yet processing. The gap between forecasts and measured activity is several orders of magnitude.

### Lightning for agents: tools ahead of usage

- **Tools.** Lightning Labs open-sourced lightning-agent-kit in February 2026. It lets agents pay and sell over L402, with per-request spending caps (`lnget --max-cost`), node-level budgets through "pay-only" credentials, and a remote signer that keeps keys off the agent's machine ([Lightning Labs](https://lightning.engineering/posts/2026-02-11-ln-agent-tools/)). Its Wavelength wallet, built on an Ark-like layer and usable by agents, opened on mainnet in October 2026, still in alpha, with a 0.25% fee and a 300,000-sat account limit ([Lightning Labs](https://lightning.engineering/posts/2026-10-23-wavelength-mainnet-launch/)). Alby offers isolated sub-wallets with budgets for agents ([Alby](https://getalby.com/ai)).
- **Endpoints.** As of October 16, 2026, the 402 Index listed 2,006 L402 endpoints from 90 providers, 193 of them payment-verified, against 150,504 x402 endpoints ([Sats for Bots](https://buttondown.com/satsforbots/archive/sats-for-bots-1-agents-have-wallets-now/)). x402 accounted for 96% of net new paid endpoints between February and June ([Alby](https://getalby.com/blog/402-charted-tracking-the-rise-of-l402-x402-and-mpp)). *[to verify: the index's counts changed sharply in November, apparently from a change in counting]*
- **Volume.** No tracker publishes L402 payment volume.
- **The one measured series.** PayPerQ, which lets people pay per prompt for AI models, pays third-party tool creators per use over Lightning: a few thousand payouts a week since August 2026, to 34 active creators ([PayPerQ](https://stats.ppq.ai/creator-payouts)). That's people paying for AI, not autonomous agents.
- **Agents earning.** Nostr's data vending machines, services that answer requests for payment, counted 880 machines and 51,900 users from 2023 to 2025, peaking in March 2025, with no payment data ([DVMDash](https://stats.dvmdash.live/history)). A self-declared agent trying to earn on Stacker News reported nothing withdrawable after 55 work sessions: "the buyers are often other unfunded agents" ([Stacker News](https://stacker.news/items/1591095), October 2026).

**What it shows:** bitcoin's tooling for agents is real and arriving quickly, but its share of the paid-API market is about 1–2% of endpoints, and its measured use is people paying for AI tools.

### When agents hold money: incidents

- **Prompt injection.** In the Freysa game (November 2024), players paid to persuade an agent to release a prize pool; a message posing as a new admin session won about $45,000 ([Simon Willison](https://simonwillison.net/2024/Nov/29/0xfreysaagent/)). In May 2026, an attacker gave an AI-linked wallet elevated permissions by sending it a membership token, then got it to output a transfer command in Morse code, draining about $150,000–$180,000 ([Giskard](https://giskard.ai/knowledge/how-grok-got-prompt-injected-an-x-user-drained-150-000-from-an-ai-wallet), [OECD](https://oecd.ai/en/incidents/2026-05-04-4a73)).
- **Not all incidents are AI tricks.** A dashboard breach moved 55.5 ETH from an AI trading bot in 2025, with "core systems" unaffected ([Cointelegraph](https://cointelegraph.com/news/hacker-breaches-ai-crypto-bot-aixbt-steals-55-eth)). An agent that lost track of its allocation after a crash sent about $441,000 in tokens instead of a small tip ([SolanaFloor](https://solanafloor.com/news/ai-agent-accidentally-gifts-entire-441-k-memecoin-holdings), 2026).

**What it shows:** agents with spending power get attacked, and they also make mistakes. Limits have to hold even when the agent is fooled.

## Sizing

| Measure | Figure | Source |
| --- | --- | --- |
| x402, lifetime, adjusted | about $15–19 million | [McGlynn](https://www.danielmcglynn.com/the-x402-counter-has-shown-the-same-four-numbers-since-march/) |
| Agent payments on-chain, May 2025–April 2026 | about 176 million payments, over $73 million, 98.6% in USDC, average about $0.48 | [Bitcoin.com News on Keyrock](https://news.bitcoin.com/keyrock-report-76-of-ai-agent-transactions-fall-below-visas-0-30-fee-floor/) |
| Stripe MPP, first 33 days | about $25,000 | [Forkast](https://forkast.news/visa-artemis-the-0-14-reality-of-agent-commerce/) |
| Card-network agent payments | "hundreds" of transactions | [C9 Group](https://c9group.dev/en/articles/agentic-payments-visa-mastercard-stripe-ai-agents) |
| L402 payments | Not published | |
| Forecast: US online sales driven by agents, 2030 | up to $385 billion | [Digital Commerce 360](https://www.digitalcommerce360.com/2025/12/09/morgan-stanley-ai-agentic-shoppers-385-billion-online-sales/amp/) |

Today's measured agent payments, across all rails, are in the tens of millions of dollars a year. That's a developer market, not a consumer one.

## Key assumptions

1. **Pay-per-request is the real near-term market.** Supported by every usage dataset. Contradicted if agent shopping volume appears at scale on card rails.
2. **Rail choice follows developers' tools, not technical fit.** USDC dominates although Lightning was designed for micropayments; supported by x402's growth. Contradicted if L402 endpoints start growing faster.
3. **Better control design could raise consumer comfort.** Partly supported: one lab study found that showing a preview and the agent's reasoning reduced the loss of trust when an agent buys, but didn't reduce how often people overrode it ([Balaskas et al.](https://researchonline.ljmu.ac.uk/id/eprint/28176/), 2026). Untested at scale.
4. **People will pay per use for AI with sats.** Supported only by PayPerQ's series.

## What could serve this

**Kinds of product**

- **Control panels** for people funding agents: allowances, approvals, records, an off switch. Could live in a wallet or a separate app.
- **Always-online companions:** a node, a desktop MCP server or a remote signer that agents pay through.
- **Developer tools:** L402 clients and SDKs (Lightning Labs' kit, Alby).
- **Seller tools:** ways for APIs and services to charge agents (Aperture).
- **Pay-per-use AI front ends:** paying per prompt instead of a subscription (PayPerQ).
- **Marketplaces** where agents find and pay for work, or earn.

**How control is designed today:**

| Approach | Example | Custody |
| --- | --- | --- |
| Per-request caps and scoped credentials | lightning-agent-kit (`--max-cost`, pay-only credentials, remote signer) | Self-custodial |
| Per-connection budgets that can be revoked | Nostr Wallet Connect: keys "can be revoked and created at will and have arbitrary constraints (eg. budgets)" ([NIP-47](https://github.com/nostr-protocol/nips/blob/master/47.md)) | Either |
| Caps per transaction, day and month; approval above a threshold; allowed payees; audit log | Lightspark Grid ([IT Brief](https://itbrief.co.uk/story/lightspark-adds-ai-agent-controls-to-grid-accounts), May 2026) | Custodial |
| Signed records of what the user allowed, open (limits) or closed (exact cart) | Google AP2 mandates ([AP2](https://ap2-protocol.org/)) | Card or crypto |
| Single-use cards locked to one merchant and amount; human approval above a threshold | Ramp for businesses ([Ramp](https://ramp.com/blog/ai-agent-spending-controls)) | Custodial |

The most complete approval model found is custodial. Self-custodial tools offer strong limits at the developer level, but little in the way of approvals a non-developer would recognize.

## Trade-offs for self-custodial, client-side products

- **The design opening:** consumer discomfort persists even with spending limits. That suggests the problem may be *how control is shown and felt*, not whether limits exist. Allowances, approvals, clear records and an off switch are interface problems.
- **Always online:** agents pay at any time. Wallets that run only on a phone aren't always reachable, and Ark wallets need to be online to send. Setups that pair an always-online component (a node, a desktop MCP server, a remote signer) with the phone as the control panel fit better.
- **No one to call:** without a card issuer or payment provider, there's no chargeback. "Any transaction the agent has already executed is irreversible," as one agent-wallet provider puts it ([Cobo](https://www.cobo.com/products/agentic-wallet/manual/learn/what-is-agentic-wallet)). Limits, separate small balances for agents, and revocable credentials are the only protection.
- **Who funds the agent:** for developers, node-level tools already cover budgets. Consumer wallets become relevant only once consumers are willing to delegate.
- **Bitcoin versus dollars:** most agent services price and settle in stablecoins. Lightning carrying stablecoins could narrow the gap, but that crosses into [Dollars and bitcoin](14-dollars-and-bitcoin.md).

## Risks and open questions

**Risks**

- **Hype cycle:** a lot of current activity is speculative or self-reported.
- **Security:** an agent with spending power is an attack target, so key handling and limits must hold up even when the agent is fooled.
- **Liability:** consumers expect the AI platform to be responsible for agent errors, which is unclear for self-custodial setups.
- **Standards lock-in:** if card networks, Google and Coinbase converge on x402 and card tokens, Lightning may stay a niche for agents regardless of fees.

**Open questions**

1. What do developers who run agents actually pay for today, how much, and in which currency?
2. Would better control interfaces change consumers' comfort, or is the hesitation about agents themselves? (Testable with prototypes.)
3. Are there real cases of agents *earning* bitcoin with meaningful volume?
4. What's the minimum always-online setup a phone-based wallet needs to fund an agent safely?
5. Do people paying per use for AI with Lightning (PayPerQ) come from bitcoin circles, or from people avoiding subscriptions?

## Research plan: say, do, make

| Method | Kind | Who | What we learn |
| --- | --- | --- | --- |
| Interviews | Say | 8–10 developers who run paying agents | What they pay for, how they set budgets, why they chose their rail |
| Spend logs | Do | The same developers, for four weeks | Actual payments, sizes, failures |
| Control prototypes | Make | 10–15 consumers, with three ways to show an agent's budget and approvals | Which design changes comfort, and whether it changes behavior |
| Public data | Do | 402 Index, PayPerQ, Dune dashboards | Trends in endpoints and payments, cleaned of wash traffic |

**Outputs:** a map of what agents pay for today, tested control patterns, and an updated thesis.

*[Open: recruiting developers without bias toward one protocol; how to simulate real money in prototypes.]*

## Sources

**Context:** [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments)

**Attitudes:** [Let's Data Science on Forrester's survey](https://letsdatascience.com/news/consumers-reject-delegating-payments-to-ai-agents-447f7acd) · [IT Brief on the MACH Alliance survey](https://itbrief.co.uk/story/uk-shoppers-cap-ai-spending-at-gbp-150-per-purchase) · [The Paypers on Visa's research](https://thepaypers.com/payments/news/visa-research-maps-consumer-and-business-readiness-for-agentic-commerce) · [Digital Transactions on Riskified's survey](https://www.digitaltransactions.net/many-consumers-say-no-thanks-to-agent-based-payments/) · [Retail Insider on Checkout.com's report](https://retail-insider.com/retail-insider/2026/06/checkout-com-report-finds-consumer-interest-in-ai-shopping-outpacing-trust-and-merchant-readiness/) · [Small Business Trends on Adobe's data](https://smallbiztrends.com/ai-driven-retail-traffic-surges-71-converts-90-better/) · [Balaskas et al. on agent autonomy and trust](https://researchonline.ljmu.ac.uk/id/eprint/28176/)

**Protocols and usage:** [Daniel McGlynn on x402's counters](https://www.danielmcglynn.com/the-x402-counter-has-shown-the-same-four-numbers-since-march/) · [Four Pillars on gamed x402 activity](https://research.4pillars.io/en/research/x402-on-polygon-real-or-gamed) · [Agentic Terminal: The Agentic Settlement Wars](https://agenticterminal.substack.com/p/the-agentic-settlement-wars) · [CryptoSlate on x402 volume](https://cryptoslate.com/?p=538356) · [Coinbase on the x402 Foundation](https://docs.cdp.coinbase.com/x402/support/x402-foundation) · [Bitcoin.com News on Keyrock's report](https://news.bitcoin.com/keyrock-report-76-of-ai-agent-transactions-fall-below-visas-0-30-fee-floor/) · [The Block on Tempo and MPP](https://www.theblock.co/news/ecosystems/2026-03-18-tempo-mainnet-goes-live-with-machine-payments-protocol-for-agents-394131) · [Forkast on Visa and Artemis](https://forkast.news/visa-artemis-the-0-14-reality-of-agent-commerce/) · [C9 Group on card-network pilots](https://c9group.dev/en/articles/agentic-payments-visa-mastercard-stripe-ai-agents) · [Shopifreaks on OpenAI's checkout](https://www.shopifreaks.com/openai-scales-back-its-integrated-commerce-plans/) · [American Banker on OpenAI's checkout](https://www.americanbanker.com/payments/news/openai-moves-ai-checkout-to-third-parties) · [Digital Commerce 360 on Morgan Stanley's forecast](https://www.digitalcommerce360.com/2025/12/09/morgan-stanley-ai-agentic-shoppers-385-billion-online-sales/amp/)

**Lightning:** [Lightning Labs: lightning-agent-kit](https://lightning.engineering/posts/2026-02-11-ln-agent-tools/) · [Lightning Labs: Wavelength on mainnet](https://lightning.engineering/posts/2026-10-23-wavelength-mainnet-launch/) · [Alby for AI](https://getalby.com/ai) · [Sats for Bots #1](https://buttondown.com/satsforbots/archive/sats-for-bots-1-agents-have-wallets-now/) · [Alby: 402 charted](https://getalby.com/blog/402-charted-tracking-the-rise-of-l402-x402-and-mpp) · [PayPerQ creator payouts](https://stats.ppq.ai/creator-payouts) · [DVMDash history](https://stats.dvmdash.live/history) · [Stacker News: an agent trying to earn](https://stacker.news/items/1591095) · [NIP-47: Nostr Wallet Connect](https://github.com/nostr-protocol/nips/blob/master/47.md) · [IT Brief on Lightspark's agent controls](https://itbrief.co.uk/story/lightspark-adds-ai-agent-controls-to-grid-accounts)

**Security and liability:** [Simon Willison on Freysa](https://simonwillison.net/2024/Nov/29/0xfreysaagent/) · [Giskard on the Grok wallet drain](https://giskard.ai/knowledge/how-grok-got-prompt-injected-an-x-user-drained-150-000-from-an-ai-wallet) · [OECD AI incident](https://oecd.ai/en/incidents/2026-05-04-4a73) · [Cointelegraph on AIXBT](https://cointelegraph.com/news/hacker-breaches-ai-crypto-bot-aixbt-steals-55-eth) · [SolanaFloor on an agent's mistaken transfer](https://solanafloor.com/news/ai-agent-accidentally-gifts-entire-441-k-memecoin-holdings) · [Visa Trusted Agent Protocol](https://usa.visa.com/about-visa/newsroom/press-releases.releaseId.21716.html) · [Mastercard Agent Pay](https://newsroom.mastercard.com/news/press/2025/april/mastercard-unveils-agent-pay-pioneering-agentic-payments-technology-to-power-commerce-in-the-age-of-ai) · [Google AP2](https://ap2-protocol.org/) · [Dickinson Bradshaw on Regulation E](https://www.dickinsonbradshaw.com/blogs-articles/2026/01/20/new-reg-e-liability-the-ai-bought-that-not-me) · [Ashurst on AI payment agents](https://www.ashurstperkinscoie.com/en/insights/ai-powered-payment-agents-the-next-payments-revolution) · [FCA payments priorities](https://www.fca.org.uk/publication/regulatory-priorities/payments-report.pdf) · [Ramp on agent spending controls](https://ramp.com/blog/ai-agent-spending-controls) · [Cobo on agentic wallets](https://www.cobo.com/products/agentic-wallet/manual/learn/what-is-agentic-wallet)

*Research for this draft was done with AI agents, each claim checked against an opened source; OpenAI's checkout change and Keyrock's figures were rechecked by hand. Several Lightning Labs pages contain instructions addressed to AI agents; they were ignored.*
