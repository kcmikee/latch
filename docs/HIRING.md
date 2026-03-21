# Latch — Team, Roles & Hiring

> $120K SCF #41 Build Award | 19-week build | June 2026 mainnet target
> 3000 Labs startup — grant is seed capital, not a payroll fund

---

## Budget Overview

| Item | Amount | Notes |
|---|---|---|
| Frontend Web Dev | $1,750 | $700/month × 2.5 months |
| Backend / SDK Dev | $1,750 | $700/month × 2.5 months |
| Designer & PM (Lexie) | $2,250 | $500/month × 4.5 months, part-time |
| Infrastructure | $4,000 | Railway, Supabase, QuickNode, tools, 5 months |
| **3000 Labs (Frankie)** | **$110,250** | Founder compensation + company capital |
| **Total** | **$120,000** | |

> Contractor pay is fair Lagos market rate (₦330K–350K/month). You built this, you won this — the company keeps the rest.

> **Confirm with SCF:** Ask if the security audit (Deliverable 6) is SCF-arranged separately. If you're paying for it yourself, audit firms charge $20–40K for Soroban contracts — factor that in.

---

## Cash Flow (Tranche Schedule)

| Tranche | Trigger | Amount | Action |
|---|---|---|---|
| T1 | Deliver D1 + D2 (~week 7) | $32,000 | Pay contractors months 1–2, infra month 1–2 |
| T2 | Deliver D3 + D4 + D5 (~week 16) | $52,000 | Pay contractors months 3–4 (final), infra month 3–4 |
| T3 | Deliver D6 + D7 + D8 (June 2026) | $36,000 | Infra month 5, 3000 Labs capital |

Pay contractors at end of each month. 30-day delay clause in agreements protects you if a tranche is late.

---

## Team

### Frankie — Founder, Tech Lead & Soroban Engineer
**Compensation:** Majority of grant as founder + 3000 Labs capital

**Owns everything hard:**
- All Rust/Soroban smart contracts (secp256k1 verifier, WebAuthn verifier, factory, bridge contract, policy hooks)
- Full contract test suite
- Relay service architecture + core logic (TypeScript/Node.js)
- SDK architecture and @latch/core spec
- Code review on all PRs
- Audit preparation and mainnet deployment

---

### Frontend Web Dev — Contract, 10 weeks
**Pay:** $700/month (~₦336K) | Total: $1,750

**Owns:**
- Latch Wallet web app (token balances, transfer history, send/receive)
- Session key management UI + policy configuration UI
- dApp interaction flow (URL-embedded XDR + refractor.space)
- Onboarding Kit UI components
- Mobile-responsive implementation
- Works from Lexie's Figma designs and Frankie's technical spec

**Must have:** React/Next.js, TypeScript, wallet integration experience (any chain)
**Nice to have:** Stellar SDK, React Native

---

### Backend / SDK Dev — Contract, 10 weeks
**Pay:** $700/month (~₦336K) | Total: $1,750

**Owns:**
- `@latch/core` TypeScript SDK
- `@latch/react` hooks (useSmartAccount, useBridge, useTransaction)
- Relay service in TypeScript/Node.js (ledger indexer, memo decoder, tx builder)
- Deployment on Railway + Supabase
- npm package publishing

**Must have:** TypeScript/Node.js, npm library experience, comfortable owning a deployment
**Nice to have:** Stellar SDK, blockchain indexing, React Native

---

### Lexie (Alexander Ejezie) — Co-founder, Designer & PM
**Relationship:** Frankie's younger brother — already named on SCF submission
**Compensation:** Equity (5–10% of 3000 Labs) + monthly stipend (TBD, family conversation)
**Not a contractor agreement — equity conversation instead**

**Owns:**
- UX design for all flows (Figma)
- SDK and developer documentation
- CEX integration guides
- Ecosystem wallet outreach materials
- Sprint planning in Linear, milestone tracking

---

## Infrastructure (No DevOps hire)

| Service | Purpose | Cost/month |
|---|---|---|
| Railway | Relay service hosting | $20–50 |
| Supabase | PostgreSQL (routing cache + tx history) | Free–$25 |
| Upstash | Redis queue (BullMQ) | $10–20 |
| QuickNode | Stellar RPC endpoint | $49–99 |
| Sentry | Error monitoring | Free tier |
| **Total** | | **~$100–200/month** |

Any backend dev can deploy on Railway. No DevOps expertise needed.

---

## Hiring Process

1. **Post** on Stellar Discord, Web3 Lagos Telegram/WhatsApp groups, Twitter/X, Talent.ng
2. **Async screen** — share the role JD and ask 3 technical questions by DM/email
3. **30-min call** — assess quality of thinking and async communication
4. **Paid task** — ₦50,000 ($100) for a 2–3 hour relevant task
5. **Contractor agreement signed → start**

Target: both hires made within 2 weeks of posting.

---

## Job Descriptions

### JD 1: Frontend Web Developer — Latch Wallet

**About Latch**
Latch is open-source infrastructure for Stellar C-address (Smart Account) onboarding, funded by the Stellar Community Fund. We're building the missing layer that lets anyone fund and use a Soroban Smart Account without needing a traditional Stellar G-address — using wallets they already have (Phantom, MetaMask, Passkeys).

**Role**
Build the Latch Wallet web app and Onboarding Kit — the entire user-facing layer of the stack. Work from Figma designs and a clear technical spec in React/Next.js, integrating with the @latch/core SDK.

**What you'll build**
- Full wallet UI: token balances, transfer history, send/receive
- 4-step onboarding flow: signer selection → C-address creation → bridge funding → ready
- Session key management and policy configuration UI
- dApp interaction (transaction signing via URL-embedded XDR + refractor.space)
- Mobile-responsive throughout

**Requirements**
- React + Next.js, TypeScript
- Web3 wallet integration (Phantom, MetaMask, WalletConnect — any chain fine)
- Figma to code, async work

**Engagement:** 10 weeks contract | $700/month | Remote | Lagos-based preferred

---

### JD 2: Backend / SDK Developer — Relay & @latch/sdk

**About Latch**
Same as above.

**Role**
Build the relay service that powers the Latch Bridge and the TypeScript SDK that every integrating wallet will use. Infrastructure-level work — clean, tested, publishable.

**What you'll build**
- `@latch/core` SDK (address derivation, memo encoding, Stellar auth helpers, verifier ABIs)
- `@latch/react` hooks (useSmartAccount, useBridge, useTransaction)
- Relay service in TypeScript/Node.js (ledger streaming, memo decoding, deposit routing, tx submission)
- Deploy on Railway + Supabase
- Publish to npm

**Requirements**
- TypeScript / Node.js production experience
- Built and published npm libraries
- Event-driven/streaming systems
- Can own a deployment on Railway or Render

**Engagement:** 10 weeks contract | $700/month | Remote | Lagos-based preferred

---

## Where to Post

| Channel | Best for |
|---|---|
| Stellar Discord `#jobs` | Stellar-native devs |
| Web3 Lagos / Lagos Tech Telegram groups | Local Lagos builders |
| Twitter/X | Motivated devs who follow the problem space |
| Talent.ng / Jobberman | Broader Lagos reach |
| SCF community channels | Ecosystem-aligned devs |
