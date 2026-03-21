# Latch — Build Plan & Team Roadmap

> SCF #41 Build Award — passed panel review 2026-03-12

---

## Immediate Actions (This Week)

- [x] Submit SCF KYC — **both** Airtable form AND Persona form (both required)
- [x] Fill out 2026 Onchain Growth Projection Form
- [ ] Do NOT share news of passing review publicly yet

---

## Reviewer Feedback — Address During Build

| # | Feedback | Action |
|---|---|---|
| 1 | **G-to-C relay trust model** — document security boundaries and failure modes | Write trust model doc: who holds keys, what happens if relay goes down, can funds get stuck, how deposits are validated |
| 2 | **Cross-ecosystem wallet signing** — WebAuthn testing surface area | Build test matrix: Chrome/Firefox/Safari × Desktop/Mobile × Phantom/MetaMask |
| 3 | **Wallet team engagement** — engage Freighter, Lobstr, xBull early | Email all three this week, before SDK design is locked |
| 4 | **URL-embedded XDR / refractor.space** — payload size and UX implications | Run demo flow with real DeFi tx (token swap, liquidity add), not just counter |

---

## Team Structure

### Minimum Viable Team (4 people)

| Role | Owns | Full-Time | Contract |
|---|---|---|---|
| **Tech Lead (you)** | Architecture, product, Soroban contracts | — | — |
| **Rust / Soroban Dev** | Bridge contract, verifiers, smart account | $120–150k/yr | $80–120/hr |
| **TypeScript Dev** | Wallet UI, SDK, Next.js, API routes | $100–130k/yr | $60–90/hr |
| **Product Designer** | Onboarding UX, wallet flows, dApp UI | $80–110k/yr | $50–80/hr |

### Add in Phase 3+

| Role | Owns |
|---|---|
| DevOps / Infra (part-time) | Relay service uptime, monitoring, bridge ops |
| React Native Dev | Mobile wallet |

### Where to Hire

- Stellar Discord + SCF alumni — best source, already know the ecosystem
- Twitter/X — post what you're building, devs will DM
- Gitcoin, Wellfound (AngelList), web3-specific boards
- Start contractors before full-time — lower risk, faster to evaluate

---

## How We Work

### Rhythm

- **Monday** — 30-min sprint planning, pick the week's goals
- **Daily** — async standup in Slack: done / doing / blocked
- **Friday** — demo anything shippable, even small wins

### Tools

| Tool | Purpose |
|---|---|
| **Linear** | Issues, sprints, roadmap |
| **GitHub Projects** | PR-linked task tracking |
| **Slack** | Async comms |
| **Notion** | Docs, architecture decisions, onboarding for new hires |

### Code Rules

- All smart contract changes require 2-person review before testnet deploy
- Bridge / relay code is security-critical — treat as money-handling code
- Feature branches → PR → review → merge, no direct pushes to main

---

## Build Roadmap

### Phase 1 — Core Demo ✅ (Complete)
- [x] Ed25519 verifier contract with prefix support
- [x] Smart Account with OZ context rules
- [x] Phantom → Smart Account demo (web)
- [x] Bundler-sponsored fee abstraction
- [x] Enforcing Mode simulation (correct Soroban signing)

### Phase 2 — Bridge & Multi-Signer
- [ ] Bridge proxy contract (G-to-C forwarding)
- [ ] Relay service (deposit monitoring + memo routing)
- [ ] secp256k1 verifier (MetaMask support)
- [ ] Passkey verifier (WebAuthn)
- [ ] Multi-signer context rules
- [ ] G-to-C relay trust model document
- [ ] WebAuthn cross-browser/cross-device test suite

### Phase 3 — Wallet & SDK
- [ ] Reference wallet (token balances, transfer history)
- [ ] `@latch/sdk` TypeScript SDK for wallet providers
- [ ] Onboarding kit — standard UX flow for wallet providers
- [ ] Mobile wallet (React Native)
- [ ] `latch-sdk` Rust SDK for contract developers

### Phase 4 — Production
- [ ] Security audit
- [ ] Audit fixes
- [ ] Mainnet deployment
- [ ] CEX integration guides
- [ ] Ecosystem wallet partnership docs

---

## SCF Form Prep

### KYC / Promotional Due Diligence
- Applying as: **Individual** (3000 Labs is not yet a registered entity)
- Legal name: **Ejezie Franklin**
- KYC link to use: Individual link — https://stellar.org/bd-kyc?y=live
- Prior KYC with SDF: No
- Tax form: **W-8BEN** (non-US individual, Nigeria)
- Stellar payment address: `GCQEHEDCWDQCRVJUUQ6TUSZ2ZTAHQBA2UMUI557J5IOZEW3RTX6UC66B`
- Memo required: No
- Address: rd3 pz estate ikorodu, Lagos, Nigeria
- Deadline: **March 17, 2026** (5 days from March 12 email)

### 2026 Onchain Growth Projections (draft)

| Metric | Projection | Notes |
|---|---|---|
| C-address deployments | TBD | Target: wallets integrating Latch SDK |
| Transaction volume | TBD | Bridge + wallet txs |
| Wallet integrations | 3 (Freighter, Lobstr, xBull) | Subject to engagement outcomes |
| SDK installs / downloads | TBD | Post-launch |

---

## Contacts

| Team | Contact | Status |
|---|---|---|
| Freighter | — | Not yet reached out |
| Lobstr | — | Not yet reached out |
| xBull | — | Not yet reached out |
| SCF Team | communityfund@stellar.org | Active |
