# Last-mile infrastructure

*Quick scan. Supporting area. Confidence: medium. Last updated November 8, 2026.*

## The question

Most of the people in the other areas need to get money in and out of bitcoin, or pay someone who doesn't use it: a supplier who takes M-Pesa or Pix, a merchant who wants USDT, a shop in Seoul that only takes won. Which pieces of that "last mile" exist today, which avoid locking users into a single provider, and what's still missing?

## What's happening

**Phone numbers are becoming payment addresses.** Since May 22, 2026, every Kenyan M-Pesa number works as a Lightning address (`phonenumber@bitcoin.co.ke`) through Tando. Payments to unclaimed numbers are converted to shillings and paid out via M-Pesa for a 1% fee, with Tando handling the funds in between. Numbers whose owners have claimed them (a one-time KES 210) receive bitcoin directly to their own wallet, with no fee ([Blink](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address)). This is close to what the [Pave](https://gbks.substack.com/p/pave-protocol-for-last-mile-bitcoin) sketch proposes, built for one country and one provider.

**Local instant-payment systems are being bridged.** BTCPay Server's DePix plugin lets customers pay a merchant with a Pix QR code, settling in DePix, a stablecoin pegged to the Brazilian real on the Liquid network ([BTCPay Server](https://blog.btcpayserver.org/depix-plugin/), September 2025).

**Swaps between bitcoin and dollars are going non-custodial.** In March 2026, Boltz launched atomic swaps between Lightning and USDT: each trade either completes on both sides or refunds both. They started on Arbitrum, with Arkade, Liquid, Rootstock and on-chain bitcoin planned ([Bitcoin Magazine](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users)). Kaleidoswap's SSPS draft goes one level up: a standard way for wallets to discover and choose between non-custodial swap providers across bitcoin layers, including Bark *[from earlier research; the repo couldn't be opened during this scan]*.

**Ark implementations handle Lightning differently.** Arkade pays Lightning invoices through a "solver" that can only claim the user's locked funds after paying the invoice ([Arkade docs](https://docs.arkadeos.com/contracts/lightning-swaps)). Bark uses Second's server as its Lightning gateway *[from memory; to verify details]*.

**Say versus do:** the ecosystem *says* "stay bitcoin-only." What working last-mile services *do* is convert at the edge, often into a local stablecoin or local money (Tando into shillings, DePix into a real-pegged token). Where conversion is invisible to the user, people don't seem to mind which rail runs underneath.

## Who

| Need | Who has it | What exists |
| --- | --- | --- |
| Pay someone on a local mobile-money or instant-payment system | Earners, group order managers, people paying suppliers | Tando (M-Pesa), DePix (Pix), and others country by country |
| Pay someone who wants stablecoins | Merchants in emerging markets (area 14) | Boltz USDT swaps, SSPS (draft) |
| Get bitcoin from fiat income | Earners (area 12) | Bitwage and similar, mostly custodial in the middle |
| Move between bitcoin layers | Any wallet user | Submarine and chain swaps (Boltz, Arkade solvers, Bark's gateway) |

## What could serve this

**Kinds of product**

- **Standards:** Pave, SSPS, Lightning addresses on phone numbers.
- **Conversion services** into local money (Tando) or local stablecoins (DePix).
- **Directories** that map phone numbers or handles to payment addresses.
- **Merchant plugins** for local payment systems (BTCPay's DePix plugin).
- **Swap providers** between bitcoin layers and assets (Boltz).

**Trade-offs for wallets**

- **Lightning addresses already reach some local systems:** a wallet that can pay a Lightning address can pay any Kenyan M-Pesa number today, with no extra integration.
- **Conversion happens at a provider,** so "self-custodial end to end" usually means the user holds their own funds while a provider briefly handles conversion. Atomic swaps narrow that gap.
- **Choice of provider is the lock-in question:** SSPS-style discovery lets a wallet avoid depending on a single swap provider. Pave aims for the same across local payment systems.
- **Design matters at the edge:** showing who receives what, in which currency, and at what cost, clearly and before the user pays.

## Risks

- **Privacy of phone numbers as payment addresses:** Brazil's Pix showed that personal identifiers as payment keys enable leaks and scams ([Sacramento](https://www.psacramento.com/pix-in-brazil-a-field-study-for-the-bitcoin-community/)). The same applies to M-Pesa numbers as Lightning addresses.

- **Regulation:** conversion into local money is regulated in most countries, and providers can disappear or change terms.
- **Fragmentation:** each country has its own system and provider, so coverage grows slowly.
- **Custody creep:** convenient services often hold funds in the middle.

## Open questions for a deep dive

1. How many payments to M-Pesa numbers via Tando happen, and do recipients claim their addresses (keep bitcoin) or take shillings?
2. What's SSPS's status, which providers have adopted it, and does it cover Bark?
3. Which countries matter most for the other areas (Korea for group orders, Brazil, Nigeria, Argentina), and what's the last-mile option in each?
4. Could Pave be built as a thin standard on top of what Tando and DePix already do?
5. What do Bark's Lightning gateway and swap options support today, and what are they missing?

## Sources

- [Blink: 40 million Kenyans now have a bitcoin Lightning address](https://blink.sv/blog/40-million-kenyans-now-have-a-bitcoin-lightning-address)
- [Pave: a protocol for last-mile bitcoin](https://gbks.substack.com/p/pave-protocol-for-last-mile-bitcoin)
- [BTCPay Server: DePix plugin](https://blog.btcpayserver.org/depix-plugin/)
- [Bitcoin Magazine on Boltz USDT swaps](https://bitcoinmagazine.com/business/boltz-exchange-launches-atomic-usdt-swaps-for-lightning-network-users)
- [Kaleidoswap SSPS](https://github.com/kaleidoswap/ssps)
- [Arkade docs: Lightning swaps](https://docs.arkadeos.com/contracts/lightning-swaps)
