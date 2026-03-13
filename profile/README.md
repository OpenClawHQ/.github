<p align="center">
  <img src="https://raw.githubusercontent.com/effectorHQ/brand-kit/main/logos/wordmark-dark.svg?v=2" alt="effectorHQ" height="72">
</p>

<p align="center"><strong>We build hands for AI that moves first.</strong></p>

<p align="center">
  <a href="https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome"></a>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="https://github.com/effectorHQ/.github/blob/main/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg" alt="Code of Conduct"></a>
  <a href="https://github.com/effectorHQ/.github/blob/main/profile/README.zh.md"><img src="https://img.shields.io/badge/文档-中文-red.svg" alt="中文文档"></a>
</p>

effectorHQ (*prev. OpenClawHQ*) is an open studio building the next generation of Proactive AI agent capabilities. Each project aims to solve a real problem, is backed by real research, and is designed to stand on its own. Together they form a coherent vision: **typed, composable, verifiable hands for AI.**

Starting with [OpenClaw](https://github.com/openclaw/openclaw), designed for a larger capability layer. We exist because one team can't cover every use case. Distributed, effector-native, community-driven is a better architecture.

We don't build the brain (that's the LLM). We don't build the body (that's the runtime — [OpenClaw](https://github.com/openclaw/openclaw), [Claude Agent SDK](https://github.com/anthropics/claude-agent-sdk-python), and whatever comes next). We build the hands — and we make sure every hand is safer, more composable, and more powerful than what existed before.

```mermaid
graph LR
  classDef brain fill:#1A1A1A,color:#F5F0EB,stroke:#1A1A1A;
  classDef body fill:#2D2D2D,color:#F5F0EB,stroke:#1A1A1A;
  classDef hands fill:#E03E3E,color:#F5F0EB,stroke:#E03E3E;

  Brain["Brain / LLMs"]:::brain --> Body["Body / Runtimes"]:::body
  Body --> Hands["Hands / Effectors"]:::hands
```

---

### The Effector Type System

> Our [analysis of 13,729 ClawHub skills](https://github.com/effectorHQ/clawhub-analysis) found a **67% agent failure rate**: driven by untyped interfaces, missing prerequisites, and permission mismatches.  
> This is the paradigm we're building: Effector = **the smallest capability unit** an agent can discover, inspect, run, compose, and carry across runtimes.

The core thesis: AI agent capabilities need types. Today you chain two skills and pray they work. Tomorrow you type-check the composition before a single token is spent.

| Project | What it is | Status |
|---------|-----------|--------|
| [`effector-spec`](https://github.com/effectorHQ/effector-spec) | **The Specification** — type language, composition algebra, discovery protocol | v0.2.0 draft |
| [`effector-types`](https://github.com/effectorHQ/effector-types) | **Standard capability types** — the `lib.d.ts` for agent tools, grounded in 13K+ skills | v0.2.0 |
| [`clawhub-analysis`](https://github.com/effectorHQ/clawhub-analysis) | **Empirical data** — 13,729 skills analyzed, type distributions, failure rates | Data + notebook |

### Quality & Tooling
`what makes capabilities reliable`

| Project | What it does | Status |
|---------|-------------|--------|
| [`skill-lint`](https://github.com/effectorHQ/skill-lint) | CLI — validate SKILL.md structure before publishing | Working (v0.2.0) |
| [`skill-eval`](https://github.com/effectorHQ/skill-eval) | **Evaluation framework** — measure whether skills actually work | v0.1.0 (static) |
| [`effector-audit`](https://github.com/effectorHQ/effector-audit) | Security audit — Sigstore signing, permission drift detection | v0.1.0 |
| [`skill-lint-action`](https://github.com/effectorHQ/skill-lint-action) | GitHub Action — inline PR annotations, zero config | Working |

### Build & Ship
`get started in minutes`

| Project | What it does | Status |
|---------|-------------|--------|
| [`create-effector`](https://github.com/effectorHQ/create-effector) | `npx create-effector` — scaffold any Effector type | Working |
| [`linear-skill`](https://github.com/effectorHQ/linear-skill) | **Reference implementation** — production-ready skill, Grade A eval, zero lint errors | v1.0.0 |
| [`plugin-template`](https://github.com/effectorHQ/plugin-template) | Skill starter template — fork and write your SKILL.md | Working |
| [`cookbook`](https://github.com/effectorHQ/cookbook) | Real-world skill recipes: Docker, Jira, PostgreSQL, git worktrees | Examples |

### Compose & Bridge
`connecting capabilities`

| Project | What it does | Status |
|---------|-------------|--------|
| [`effector-compose`](https://github.com/effectorHQ/effector-compose) | Build agent pipelines, type-check them, emit to any runtime | Early |
| [`effector-graph`](https://github.com/effectorHQ/effector-graph) | Capability graph visualization and path-finding | Early |
| [`openclaw-mcp`](https://github.com/effectorHQ/openclaw-mcp) | SKILL.md → MCP bridge — make skills work in Claude, Cursor, Windsurf | v0.1.0 |

### Explore & Learn

| Project | What it does |
|---------|-------------|
| [`awesome-openclaw`](https://github.com/effectorHQ/awesome-openclaw) | Curated list of skills, extensions, tools, and resources |
| [`workspace-templates`](https://github.com/effectorHQ/workspace-templates) | Agent persona bundles (DevOps, Code Reviewer, Security Auditor) |
| [`lobster-recipes`](https://github.com/effectorHQ/lobster-recipes) | Workflow pipelines: deploy-and-notify, daily-standup, PR-review-triage |
| [`docs`](https://github.com/effectorHQ/docs) | Community guides: architecture, skill development, extension development |

### Prev.

| Project | What it does |
|---------|-------------|
| [`OpentheClaw`](https://github.com/effectorHQ/OpentheClaw) | One‑click SSH tunnel + Web login |
| [`free-search-proxy`](https://github.com/OpenClawHQ/free-search-proxy) | DuckDuckGo‑based search proxy API for OpenClaw agents |

### Governance

| Document | Purpose |
|----------|---------|
| [`manifesto`](https://github.com/effectorHQ/manifesto) | Founding theses — why typed capabilities matter |
| [`rfcs`](https://github.com/effectorHQ/rfcs) | RFC process for spec changes and new products |
| [Contributing Guide](https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md) | How to contribute to any project |

---

### What gets built here

| Effector Type | What it is |
|---------------|-----------|
| **Skill Effectors** | Markdown-defined capabilities (SKILL.md) with typed interfaces |
| **Extension Effectors** | TypeScript plugins that hook into runtime SDKs |
| **Workflow Effectors** | Multi-step pipelines with typed composition |
| **Workspace Effectors** | Agent persona bundles (SOUL.md, AGENTS.md, TOOLS.md) |
| **Bridge Effectors** | Cross-runtime adapters (OpenClaw ↔ MCP ↔ others) |
| **Quality Effectors** | Lint, eval, audit, and supply-chain tools |

### How we build

| Principle | In practice |
|-----------|-------------|
| **Demo First** | Ship working code before writing proposals. A running prototype beats a perfect spec. |
| **Ship Loud** | Every merge, every release note, every contributor gets signal. Shipping should feel like winning. |
| **Open by Default** | Code, roadmap, decisions, failed experiments — if it can be open, it is. |

---

### Join the build

This is a community project. No gatekeeping. Browse a repo, open a PR, or start something new.

If you have questions, open an issue in the relevant repo or start a [Discussion](https://github.com/orgs/effectorHQ/discussions).

---

<sub>Every effector extends the reach. © 2026 effectorHQ Contributors</sub>
