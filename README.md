# vorionsys

**Governance infrastructure for autonomous AI agents.**

We build open primitives -- trust scoring, policy enforcement, cryptographic audit trails --
so AI agents can earn autonomy instead of being granted it blindly.

**Alex Blanc** - Intent & enforcement  |  **Ryan Cason (Bo Xandar Lee)** - Trust scoring & audit trails

---

### What we're building

| Repo | What it does | |
|---|---|---|
| [**vorion**](https://github.com/vorionsys/vorion) | Full governance monorepo — BASIS standard, ATSF scoring, CAR registry, SDKs | 13,600+ tests · Apache 2.0 |
| [**cognigate**](https://github.com/vorionsys/cognigate) | Enforcement runtime: INTENT → ENFORCE → PROOF | 692 tests · Live at [cognigate.dev](https://cognigate.dev) |

---

### Published packages

**Foundation**

| Package | Version | Description |
|---|---|---|
| [@vorionsys/shared-constants](https://www.npmjs.com/package/@vorionsys/shared-constants) | [![npm](https://img.shields.io/npm/v/@vorionsys/shared-constants?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/shared-constants) | Canonical trust tiers, role mappings, provenance types |
| [@vorionsys/contracts](https://www.npmjs.com/package/@vorionsys/contracts) | [![npm](https://img.shields.io/npm/v/@vorionsys/contracts?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/contracts) | Zod schemas, Drizzle DB table definitions, shared validators |
| [@vorionsys/basis](https://www.npmjs.com/package/@vorionsys/basis) | [![npm](https://img.shields.io/npm/v/@vorionsys/basis?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/basis) | BASIS rule engine -- 182-day stepped trust decay, 8-tier scoring |
| [@vorionsys/atsf-core](https://www.npmjs.com/package/@vorionsys/atsf-core) | [![npm](https://img.shields.io/npm/v/@vorionsys/atsf-core?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/atsf-core) | ATSF trust scoring framework |
| [@vorionsys/car-spec](https://www.npmjs.com/package/@vorionsys/car-spec) | [![npm](https://img.shields.io/npm/v/@vorionsys/car-spec?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/car-spec) | CAR (Categorical Agentic Registry) specification v1.1.0 |

**Governance & Enforcement**

| Package | Version | Description |
|---|---|---|
| [@vorionsys/cognigate](https://www.npmjs.com/package/@vorionsys/cognigate) | [![npm](https://img.shields.io/npm/v/@vorionsys/cognigate?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/cognigate) | Cognigate policy enforcement SDK |
| [@vorionsys/council](https://www.npmjs.com/package/@vorionsys/council) | [![npm](https://img.shields.io/npm/v/@vorionsys/council?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/council) | 16-agent governance orchestrator |
| [@vorionsys/ai-gateway](https://www.npmjs.com/package/@vorionsys/ai-gateway) | [![npm](https://img.shields.io/npm/v/@vorionsys/ai-gateway?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/ai-gateway) | AI provider gateway with policy enforcement |
| [@vorionsys/proof-plane](https://www.npmjs.com/package/@vorionsys/proof-plane) | [![npm](https://img.shields.io/npm/v/@vorionsys/proof-plane?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/proof-plane) | Dual-hash (SHA-256 + SHA3-256) tamper-evident audit chain |
| [@vorionsys/security](https://www.npmjs.com/package/@vorionsys/security) | [![npm](https://img.shields.io/npm/v/@vorionsys/security?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/security) | Crypto, DPoP, and Merkle modules |

**SDKs & Clients**

| Package | Version | Description |
|---|---|---|
| [@vorionsys/sdk](https://www.npmjs.com/package/@vorionsys/sdk) | [![npm](https://img.shields.io/npm/v/@vorionsys/sdk?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/sdk) | Platform SDK for building on Vorion |
| [@vorionsys/agent-sdk](https://www.npmjs.com/package/@vorionsys/agent-sdk) | [![npm](https://img.shields.io/npm/v/@vorionsys/agent-sdk?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/agent-sdk) | Agent-facing SDK for governance integration |
| [@vorionsys/runtime](https://www.npmjs.com/package/@vorionsys/runtime) | [![npm](https://img.shields.io/npm/v/@vorionsys/runtime?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/runtime) | Agent runtime environment |
| [@vorionsys/platform-core](https://www.npmjs.com/package/@vorionsys/platform-core) | [![npm](https://img.shields.io/npm/v/@vorionsys/platform-core?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/platform-core) | Trust engine, governance, enforcement, and proof integration |
| [@vorionsys/car-client](https://www.npmjs.com/package/@vorionsys/car-client) | [![npm](https://img.shields.io/npm/v/@vorionsys/car-client?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/car-client) | CAR API client library |
| [@vorionsys/car-cli](https://www.npmjs.com/package/@vorionsys/car-cli) | [![npm](https://img.shields.io/npm/v/@vorionsys/car-cli?label=&color=blue)](https://www.npmjs.com/package/@vorionsys/car-cli) | CAR CLI tooling for agent registry management |

```bash
npm install @vorionsys/shared-constants   # start here
```

---

### Standards alignment

- **NIST AI RMF** — ~86% coverage across Govern, Map, Measure, Manage
- **NIST SP 800-53** — 370 controls in OSCAL SSP (OSCAL 1.1.2, validated)
- **NIST CAISI** — RFI response pending submission, Docket NIST-2025-0035, deadline March 9, 2026
- **OWASP ASI** — Top 10 for Agentic Applications (ASI01–ASI10) mapped
- **ISO/IEC 42001** — Gap analysis complete

---

### Our story (the short version)

We both spent years serving banquets -- long nights, heavy trays, plenty of time to think.
College didn't stick; the pace couldn't match our minds. Then AI arrived and everything clicked.

We started building projects separately. Both hit the same wall: LLMs create a rocky,
ever-changing surface. You build something solid one day and the next it needs constant propping up.
It felt like constructing on sand.

So we combined our work -- intent/enforcement + trust/audit -- into Vorion.
Our small offering to the community.

We believe AI is humanity's greatest asset in the making, but it won't happen by chance.
It must be guided.

[About & Manifesto ->](https://vorion.org/manifesto) - [vorion.org](https://vorion.org) - [cognigate.dev](https://cognigate.dev) - hello@vorion.org

---

*We're just getting started. Feedback welcome -- even the brutal kind.*
