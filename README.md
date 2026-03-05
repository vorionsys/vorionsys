# vorionsys

**Governance infrastructure for autonomous AI agents.**

We build open primitives — trust scoring, policy enforcement, cryptographic audit trails —
so AI agents can earn autonomy instead of being granted it blindly.

**Alex Blanc** · Intent & enforcement &nbsp;|&nbsp; **Ryan Cason (Bo Xandar Lee)** · Trust scoring & audit trails

---

### What we're building

| Repo | What it does | |
|---|---|---|
| [**vorion**](https://github.com/vorionsys/vorion) | Full governance monorepo — BASIS standard, ATSF scoring, CAR registry, SDKs | 10,668+ tests · Apache 2.0 |
| [**cognigate**](https://github.com/vorionsys/cognigate) | Enforcement runtime: INTENT → ENFORCE → PROOF | 692 tests · Live at [cognigate.dev](https://cognigate.dev) |

---

### Published packages

| Package | Description |
|---|---|
| [`@vorionsys/shared-constants`](https://www.npmjs.com/package/@vorionsys/shared-constants) | Canonical trust tiers, role mappings, provenance types |
| [`@vorionsys/contracts`](https://www.npmjs.com/package/@vorionsys/contracts) | Zod schemas, Drizzle DB table definitions, shared validators |
| [`@vorionsys/basis`](https://www.npmjs.com/package/@vorionsys/basis) | BASIS rule engine — 182-day stepped trust decay, 8-tier scoring |
| [`@vorionsys/atsf-core`](https://www.npmjs.com/package/@vorionsys/atsf-core) | ATSF trust scoring framework |
| [`@vorionsys/car-spec`](https://www.npmjs.com/package/@vorionsys/car-spec) | CAR (Categorical Agentic Registry) specification v1.1.0 |
| [`@vorionsys/cognigate`](https://www.npmjs.com/package/@vorionsys/cognigate) | Cognigate enforcement SDK |

```bash
npm install @vorionsys/shared-constants   # start here
```

---

### Standards alignment

- **NIST AI RMF** — ~86% coverage across Govern, Map, Measure, Manage
- **NIST SP 800-53** — 370 controls in OSCAL SSP (OSCAL 1.1.2, validated)
- **NIST CAISI** — RFI response submitted, Docket NIST-2025-0035, March 2026
- **OWASP ASI** — Top 10 for Agentic Applications (ASI01–ASI10) mapped
- **ISO/IEC 42001** — Gap analysis complete

---

### Our story (the short version)

We both spent years serving banquets — long nights, heavy trays, plenty of time to think.
College didn't stick; the pace couldn't match our minds. Then AI arrived and everything clicked.

We started building projects separately. Both hit the same wall: LLMs create a rocky,
ever-changing surface. You build something solid one day and the next it needs constant propping up.
It felt like constructing on sand.

So we combined our work — intent/enforcement + trust/audit — into Vorion.
Our small offering to the community.

We believe AI is humanity's greatest asset in the making, but it won't happen by chance.
It must be guided.

[About & Manifesto →](https://vorion.org/manifesto) · [vorion.org](https://vorion.org) · [cognigate.dev](https://cognigate.dev) · hello@vorion.org

---

*We're just getting started. Feedback welcome — even the brutal kind.*
