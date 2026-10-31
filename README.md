# AiGhost — Investor & Technology Overview

**Local-first AI direction, privacy-first social software, and opt-in home-node infrastructure**  
*Public overview only — the core source code remains private.*

## What AiGhost is

AiGhost is a software ecosystem being developed around a privacy-first social and messaging application, user-controlled local intelligence, and an opt-in network of home nodes. The project also contains an isolated software research prototype called **Neuroplasma Optical Fabric**, which models selected ideas for optical transport, active processing, routing, temporary buffering, and persistent memory.

The project is best understood as three connected development tracks:

1. **Ghost application** — a privacy-first social and messaging product.
2. **Ghost Home Node** — a consent-based, same-account store-and-forward system for enrolled devices.
3. **Neuroplasma Optical Fabric** — an isolated software model exploring a future hybrid optical/electronic network architecture.

## What exists today

| Area | Evidence-backed description | Boundary |
|---|---|---|
| Ghost application | Existing application codebase and product modules | This overview does not certify every route or production deployment. |
| Home Node | Consent-gated node registry and bounded packet queue are documented in the repository | Current pilot is limited to opted-in nodes belonging to the same account; it is not a public VPN, proxy, or general file network. |
| Local intelligence | The development architecture specifies local inference and local memory as the preferred path | Availability depends on the configured host and model; do not assume every device is independently capable. |
| Neuroplasma | Software models, diagnostics, and focused regression tests exist in the development branch | Physical optical transport and fibre hardware are not connected. Numerical demonstrations are simulated, not hardware measurements. |

## Why it may matter

AiGhost explores a product direction in which useful AI and network capabilities are closer to the user and their devices, with explicit consent and bounded participation rather than silently treating personal devices as shared infrastructure.

Neuroplasma extends that research direction into a testable software model. It keeps optical transport, active optical processing, temporary signal delay, and persistent memory as separate engineering concepts. This distinction is important: ordinary fibre and passive mirrors do not behave like general-purpose computer memory or software processors.

## What we are looking for

The project is open to exploratory discussions about:

- product and pilot partnerships;
- technical collaboration on local-first software and opt-in node clients;
- qualified laboratory collaboration for physical optical research;
- software licensing or strategic technology discussions, subject to ownership and legal due diligence.

No price, valuation, equity allocation, token terms, return, or investment instrument is offered in this public overview.

## Evidence and limitations

The repository's Neuroplasma engineering note dated 2026-10-30 describes an isolated five-role software loopback and records focused tests. It explicitly states that no physical transceiver, fibre, NIC, or live optical transport was used. The same note says key provisioning, secure distribution, rotation, and recovery are not yet implemented.

The latest inspected development commit is `f82532cc47c3ad620cd2b36202940f1507dcbbd1` on `feat/ghost-home-node-self-dev` (2026-10-31). The GitHub status endpoint showed three Vercel checks failing with the description **“Account is blocked.”** No current passing check-run set was returned for that commit. Production availability is therefore not claimed here.

## Source-code and access policy

The production/development source repositories remain private. This public overview is not a source-code release and grants no software licence. Detailed technical diligence, if appropriate, should use a separately agreed, time-limited process after ownership, contributor rights, and confidentiality requirements have been reviewed.

**Do not add source files, secrets, private keys, node tokens, customer data, infrastructure addresses, or internal deployment configuration to a public showcase.**

## Next step

For a technical walkthrough or a non-binding partnership discussion, contact the project owner through the [GitHub profile](https://github.com/karuott888999-ui).

---

*This document is an informational technology overview only. It is not an offer or invitation to buy or subscribe for shares, securities, tokens, loans, or any other financial product; it is not investment advice; and it contains no promise of financial return. Any future financing or commercial agreement would require separate legal, corporate, technical, and financial review.*
