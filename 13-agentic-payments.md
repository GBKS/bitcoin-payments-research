# Agentic payments

*Quick scan. Confidence: medium on the market, low on what people want. Last updated November 8, 2026.*

## The question

AI agents need small, programmable payments, which Lightning was built for. Yet the first agent payment tools settle mostly in stablecoins. Is there real demand for agent payments today, from whom, and would people actually hand an agent a budget?

## What's happening

**Developers are building; consumers are hesitant.**

- **x402 leads, but early volume was hype.** Coinbase's x402 is the most used agent payment protocol, and about 99% of its payments are in USDC ([Spiral report](https://github.com/spiralxyz/bitcoin-payments)). One analysis counts more than 50 million cumulative x402 transactions, but daily volume fell 92%, from a peak of about 731,000 in December 2025 to about 57,000 ([Agentic Terminal](https://agenticterminal.substack.com/p/the-agentic-settlement-wars)).
- **L402 is small but growing.** As of October 16, 2026, the 402 Index listed 2,006 L402 endpoints from 90 providers, 193 of them payment-verified, against 150,504 x402 endpoints ([Sats for Bots](https://buttondown.com/satsforbots/archive/sats-for-bots-1-agents-have-wallets-now/)).
- **The big platforms are choosing other rails.** Google's AP2 supports stablecoins through x402, Stripe's Machine Payments Protocol charges agents per API call, and Meta's Muse launched with PayPal and Shop Pay, not bitcoin ([Spiral report](https://github.com/spiralxyz/bitcoin-payments)).
- **The bitcoin tooling now exists.** Lightning Labs open-sourced lightning-agent-kit in February 2026. It lets agents pay and sell over L402, with per-request spending caps (`lnget --max-cost`), node-level budgets through "pay-only" credentials, and a remote signer that keeps keys off the agent's machine ([Lightning Labs](https://lightning.engineering/posts/2026-02-11-ln-agent-tools/)).

**Consumers don't want agents to pay yet.**

- In Forrester's April 2026 survey of online adults in the US, UK and Canada, three-quarters were uncomfortable letting an agent buy and pay on its own, **even when they could set spending limits and rules in advance**. A minority would accept it for routine, low-cost purchases under strict thresholds ([Let's Data Science on Forrester](https://letsdatascience.com/news/consumers-reject-delegating-payments-to-ai-agents-447f7acd), June 2026).
- In a MACH Alliance survey of more than 1,000 UK consumers, only 9% were comfortable with AI completing a payment for them. On average, they'd let AI spend about £149 per purchase ([IT Brief](https://itbrief.co.uk/story/uk-shoppers-cap-ai-spending-at-gbp-150-per-purchase), September 2026).

**Say versus do:** builders talk about an agent economy, but measured activity is small and partly speculative (x402's 92% drop). Consumers *say* they won't delegate payments. Developers *do* pay for APIs through agents, which is where real usage is.

## Who

| Group | Role | Notes |
| --- | --- | --- |
| Developers running agents | Fund agents that pay per API call or per request | The real users today; want programmatic budgets, not apps |
| API and service providers | Earn from agents (L402 tools such as Aperture) | The "agents earning" side; overlaps with area 12 |
| Agents themselves | Earn for useful work, pass value on | Mostly experiments so far *[to verify: real examples with volume]* |
| Consumers | Delegate small, routine purchases | Hesitant; control and trust are the barrier |

## What could serve this

**Kinds of product**

- **Control panels** for people funding agents: allowances, approvals, records, an off switch. Could live in a wallet or a separate app.
- **Always-online companions:** a node, a desktop MCP server or a remote signer that agents pay through.
- **Developer tools:** L402 clients and SDKs (Lightning Labs' kit).
- **Seller tools:** ways for APIs and services to charge agents (Aperture).
- **Marketplaces** where agents find and pay for work, or earn.

**Trade-offs for wallets**

- **The design opening:** consumer discomfort persists even with spending limits. That suggests the problem may be *how control is shown and felt*, not whether limits exist. Allowances, approvals, clear records and an off switch are interface problems.
- **Always online:** agents pay at any time. Wallets that run only on a phone aren't always reachable, and Ark wallets need to be online to send. Setups that pair an always-online component (a node, a desktop MCP server, a remote signer) with the phone as the control panel fit better.
- **Who funds the agent:** for developers, node-level tools already cover budgets. Consumer wallets become relevant only once consumers are willing to delegate.
- **Bitcoin versus dollars:** most agent services price and settle in stablecoins. Lightning carrying stablecoins (Taproot Assets) could narrow the gap, but that crosses into area 14.

## Risks

- **Hype cycle:** a lot of current activity is speculative.
- **Security:** an agent with spending power is an attack target, so key handling and limits must hold up.
- **Liability:** consumers expect the AI platform to be responsible for agent errors, which is unclear for self-custodial setups.

## Open questions for a deep dive

1. What do developers who run agents actually pay for today, how much, and in which currency?
2. Would better control interfaces change consumers' comfort, or is the hesitation about agents themselves? (Testable with prototypes.)
3. Are there real cases of agents *earning* bitcoin with meaningful volume?
4. What's the minimum always-online setup a phone-based wallet needs to fund an agent safely?
5. Where do agent payments meet the other areas: creators paid per use (16), API sellers earning (12)?

## Sources

- [Spiral: The Long Road to Bitcoin Payments](https://github.com/spiralxyz/bitcoin-payments)
- [Agentic Terminal: The Agentic Settlement Wars](https://agenticterminal.substack.com/p/the-agentic-settlement-wars)
- [Sats for Bots #1: Agents have wallets now](https://buttondown.com/satsforbots/archive/sats-for-bots-1-agents-have-wallets-now/)
- [Lightning Labs: lightning-agent-kit](https://lightning.engineering/posts/2026-02-11-ln-agent-tools/)
- [Let's Data Science on Forrester's survey](https://letsdatascience.com/news/consumers-reject-delegating-payments-to-ai-agents-447f7acd)
- [IT Brief on the MACH Alliance survey](https://itbrief.co.uk/story/uk-shoppers-cap-ai-spending-at-gbp-150-per-purchase)
