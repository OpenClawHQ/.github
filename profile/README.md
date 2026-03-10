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

Currently powering the [OpenClaw](https://github.com/openclaw/openclaw) ecosystem.
We exist because one team can't cover every use case. Distributed, effector-native, community-driven is a better architecture.

We don't build the brain (that's the LLM). We don't build the body (that's the runtime — [OpenClaw](https://github.com/openclaw/openclaw), Claude Agent SDK, and whatever comes next). We build the hands — and we make sure every hand is safer, more composable, and more powerful than what existed before.

---

### The Effector Type System

The core thesis: AI agent capabilities need types. Today you chain two skills and pray they work. Tomorrow you type-check the composition before a single token is spent. This is the paradigm we're building.

| Project | What it is |
|---------|-----------|
| [`effector-spec`](https://github.com/effectorHQ/effector-spec) | **The Effector Specification** — type language, composition algebra, discovery protocol. The flagship. |
| [`effector-types`](https://github.com/effectorHQ/effector-types) | **Standard capability types** — the `lib.d.ts` for AI agent tools. Input types, output types, context types. |
| [`effector-compose`](https://github.com/effectorHQ/effector-compose) | **Composition engine** — build agent pipelines, type-check them, emit to any runtime. |
| [`effector-graph`](https://github.com/effectorHQ/effector-graph) | **Capability graph visualization** — interactive explorer for the typed capability network. |
| [`effector-audit`](https://github.com/effectorHQ/effector-audit) | **Security audit + signing** — Sigstore-based signing, static analysis, supply chain verification. |

### Build & Ship

| Project | What it does |
|---------|-------------|
| [`create-effector`](https://github.com/effectorHQ/create-effector) | `npx create-effector` — scaffold any Effector type in seconds |
| [`plugin-template`](https://github.com/effectorHQ/plugin-template) | Skill starter template — fork and write your SKILL.md |
| [`cookbook`](https://github.com/effectorHQ/cookbook) | Real-world skill recipes: Notion, Docker, Jira, PostgreSQL, git worktrees |
| [`linear-skill`](https://github.com/effectorHQ/linear-skill) | Reference implementation — production-ready skill, zero lint errors |

### Quality & Tooling

| Project | What it does |
|---------|-------------|
| [`skill-lint`](https://github.com/effectorHQ/skill-lint) | CLI — validate your SKILL.md before publishing |
| [`skill-lint-action`](https://github.com/effectorHQ/skill-lint-action) | GitHub Action — inline PR annotations, zero config |
| [`openclaw-mcp`](https://github.com/effectorHQ/openclaw-mcp) | SKILL.md → MCP bridge — make skills work in Claude, Cursor, Windsurf |

### Explore & Learn

| Project | What it does |
|---------|-------------|
| [`awesome-openclaw`](https://github.com/effectorHQ/awesome-openclaw) | Curated list of skills, extensions, tools, and resources |
| [`workspace-templates`](https://github.com/effectorHQ/workspace-templates) | Agent persona bundles (DevOps, Code Reviewer, Security Auditor, etc.) |
| [`lobster-recipes`](https://github.com/effectorHQ/lobster-recipes) | Workflow pipelines: deploy-and-notify, daily-standup, PR-review-triage |
| [`docs`](https://github.com/effectorHQ/docs) | Community guides: architecture, skill development, extension development |

### Governance

| Document | Purpose |
|----------|---------|
| [`manifesto`](https://github.com/effectorHQ/manifesto) | Founding theses — why typed capabilities matter |
| [`rfcs`](https://github.com/effectorHQ/rfcs) | RFC process for spec changes and new products |
| [Contributing Guide](https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md) | How to contribute to any project |

---

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
