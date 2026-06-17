# Vorion — open infrastructure for AI agent governance

> **BASIS is to AI-agent governance what OAuth is to delegated authorization — an open standard so an agent trusted by one system can be evaluated by another.**

**BASIS — the open standard for trustworthy AI agents.** Vorion builds the open spec, the enforcement engine, and the developer tools that let any system decide — in real time — whether an AI agent's action should run, and emit cryptographic proof of *why*.

> 📍 You're on **@vorionsys** — the home of Vorion's published open-source packages (`@vorionsys/*` on npm, Apache-2.0). Website: **[vorion.org](https://vorion.org)** · Spec: **[basis.vorion.org](https://basis.vorion.org)** · Learn: **[learn.vorion.org](https://learn.vorion.org)**

### The ecosystem at a glance

```
BASIS spec (the standard)             →  basis-spec · car-spec
  └─ real-time enforcement pipeline   →  basis-gate (spec · industry · runtime)
       └─ build on it                 →  sdk · contracts · shared-constants
            └─ use it where you work  →  MCP server · vorion-find CLI
                 └─ enterprise         →  AgentAnchor · Cognigate (vorion.org)
```

### Start here

- **Read the standard** → [basis.vorion.org](https://basis.vorion.org) · spec repo [`basis-spec`](https://github.com/vorionsys/basis-spec)
- **Enforce it in code** → [`basis-gate`](https://github.com/vorionsys/basis-gate) — `npm i @vorionsys/basis-gate-runtime` (+ `-spec`, `-industry`)
- **Integrate via the SDK** → [`sdk`](https://github.com/vorionsys/sdk) — TypeScript client
- **Use it in your tools** → [Vorion MCP server](https://github.com/voriongit/mcp-server) (Claude Desktop & MCP clients) · [vorion-find](https://github.com/voriongit/vorion-find) (scan a device for AI agents)
- **Contribute** → start in [`basis-gate`](https://github.com/vorionsys/basis-gate) (`CONTRIBUTING` · `CODE_OF_CONDUCT` · `SECURITY`)
- **Roadmap** → [`basis-gate` ROADMAP](https://github.com/vorionsys/basis-gate/blob/main/ROADMAP.md) — where the open core is headed
- **Enterprise governance** → [vorion.org](https://vorion.org) (AgentAnchor, Cognigate)

### Core repositories — Apache-2.0

| Repo | What it is | Install |
|---|---|---|
| [`basis-spec`](https://github.com/vorionsys/basis-spec) | The BASIS open standard — canonical trust formulas, tiers, and types | `@vorionsys/basis-spec` |
| [`basis-gate`](https://github.com/vorionsys/basis-gate) | Real-time governance pipeline: spec + industry profiles + runtime, with two-stage proof chains | `@vorionsys/basis-gate-runtime` · `-spec` · `-industry` |
| [`car-spec`](https://github.com/vorionsys/car-spec) | OpenAPI 3.1 spec for the Categorical Agentic Registry (CAR) + Trust Engine API | *spec — not on npm* |
| [`sdk`](https://github.com/vorionsys/sdk) | TypeScript client for AI agent governance | `@vorionsys/sdk` |
| [`contracts`](https://github.com/vorionsys/contracts) | Shared Zod schemas, TypeScript types, and validators | `@vorionsys/contracts` |
| [`shared-constants`](https://github.com/vorionsys/shared-constants) | Tiers, domains, capabilities, rate limits, error codes | `@vorionsys/shared-constants` |

### Tools & related repos

- [`mcp-server`](https://github.com/voriongit/mcp-server) — Model Context Protocol server exposing local trust governance + remote Cognigate runtime tools.
- [`vorion-find`](https://github.com/voriongit/vorion-find) — zero-dep CLI that scans a device for AI agents and streams findings.
- [`rainbow`](https://github.com/voriongit/rainbow) — windowed non-binary orchestration analytics (`@vorionsys/rainbow`).
- [`basis-spec-docs`](https://github.com/voriongit/basis-spec-docs) — the BASIS documentation site (powers basis.vorion.org).

### How the repos are organized

- **`@vorionsys`** (here) — the published open-source **packages & specs** you install from npm.
- **[`voriongit`](https://github.com/voriongit)** — Vorion's GitHub **organization**: the development monorepo and several of the tools above (MCP server, CLI, analytics), linked from here.
- Everything public is **Apache-2.0**. The enterprise products (AgentAnchor, Cognigate) build on this open core — see [vorion.org](https://vorion.org).

---

*BASIS = Baseline Authority for Safe & Interoperable Systems. © Vorion LLC · Apache-2.0.*

<!--
MANUAL RESIDUAL ITEMS (GitHub web-UI only — not editable via this README):
  1. Set the @vorionsys account bio (Settings → Profile → Bio).
  2. Pin the 6 canonical repos on the profile: basis-spec, basis-gate, car-spec, sdk, contracts, shared-constants
     (profile page → "Customize your pins").
-->
