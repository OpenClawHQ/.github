<p align="center">
  <img src="https://raw.githubusercontent.com/effectorHQ/brand-kit/main/logos/wordmark-dark.svg?v=2" alt="effectorHQ" height="72">
</p>

<p align="center"><strong>为 AI 打造双手，先做再说。</strong></p>

<p align="center">
  <a href="https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="欢迎 PR"></a>
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="https://github.com/effectorHQ/.github/blob/main/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg" alt="行为准则"></a>
  <a href="./README.md"><img src="https://img.shields.io/badge/docs-English-blue.svg" alt="English"></a>
</p>

---

effectorHQ 是一个开放工作室，构建下一代 AI agent 能力基础设施。每个项目都是独立的产品——解决一个真实问题，有研究支撑，能独立被引用和采用。所有产品共同构成一个愿景：**为 AI 打造有类型、可组合、可验证的双手。**

我们不做大脑（那是 LLM 的事）。我们不做身体（那是 runtime 的事——[OpenClaw](https://github.com/openclaw/openclaw)、Claude Agent SDK、以及未来的一切）。我们做手——并且确保每一只手都比之前更安全、更可组合、更强大。

---

### Effector 类型系统

核心论点：AI agent 能力需要类型系统。今天你把两个 skill 串起来然后祈祷它能跑。明天你在第一个 token 花出去之前就完成类型检查。这就是我们在构建的范式。

| 项目 | 定位 |
|------|------|
| [`effector-core`](https://github.com/effectorHQ/effector-core) | **共享内核** — TOML/SKILL 解析、类型检查、schema 校验、跨 runtime 编译（`@effectorhq/core`）。 |
| [`effector-spec`](https://github.com/effectorHQ/effector-spec) | **Effector 规范** — 类型语言、组合代数、发现协议。旗舰项目。 |
| [`effector-types`](https://github.com/effectorHQ/effector-types) | **标准能力类型库** — AI agent 工具的 `lib.d.ts`（`@effectorhq/types`），包括输入/输出/上下文类型。 |
| [`effector-compose`](https://github.com/effectorHQ/effector-compose) | **组合引擎** — 构建 agent 管道、类型检查、输出到任意 runtime（`@effectorhq/compose`）。 |
| [`effector-graph`](https://github.com/effectorHQ/effector-graph) | **能力图谱可视化** — 类型化能力网络的交互式浏览器（`@effectorhq/graph`）。 |
| [`effector-audit`](https://github.com/effectorHQ/effector-audit) | **安全审计** — 静态扫描 + 权限漂移检测（`@effectorhq/audit`）。 |

### 构建 & 发布

| 项目 | 用途 |
|------|------|
| [`create-effector`](https://github.com/effectorHQ/create-effector) | `npx @effectorhq/create-effector` — 秒级脚手架，支持所有 Effector 类型 |
| [`plugin-template`](https://github.com/effectorHQ/plugin-template) | Skill 启动模板（计划并入 create-effector） |
| [`cookbook`](https://github.com/effectorHQ/cookbook) | 实战食谱：Notion、Docker、Jira、PostgreSQL、git worktrees |
| [`linear-skill`](https://github.com/effectorHQ/linear-skill) | 参考实现 — 生产就绪，零 lint 错误 |

### 质量 & 工具链

| 项目 | 用途 |
|------|------|
| [`skill-lint`](https://github.com/effectorHQ/skill-lint) | CLI — 发布前验证你的 SKILL.md（`npx @effectorhq/skill-lint`） |
| [`skill-lint-action`](https://github.com/effectorHQ/skill-lint-action) | GitHub Action — PR 内联标注，零配置（`@effectorhq/skill-lint-action`） |
| [`openclaw-mcp`](https://github.com/effectorHQ/openclaw-mcp) | SKILL.md → MCP 桥接 — 让 skill 在 Claude、Cursor、Windsurf 中工作 |

### 探索 & 学习

| 项目 | 用途 |
|------|------|
| [`awesome-openclaw`](https://github.com/effectorHQ/awesome-openclaw) | 精选列表：技能、扩展、工具、资源 |
| [`workspace-templates`](https://github.com/effectorHQ/workspace-templates) | Agent 人格套件（DevOps、Code Reviewer、Security Auditor 等） |
| [`lobster-recipes`](https://github.com/effectorHQ/lobster-recipes) | 工作流管道：部署通知、每日站会、PR 审查分流 |
| [`docs`](https://github.com/effectorHQ/docs) | 社区指南：架构、skill 开发、扩展开发 |

### 治理

| 文档 | 用途 |
|------|------|
| [`manifesto`](https://github.com/effectorHQ/manifesto) | 创始论纲 — 为什么类型化能力很重要 |
| [`rfcs`](https://github.com/effectorHQ/rfcs) | RFC 流程 — 规范变更和新产品提案 |
| [贡献指南](https://github.com/effectorHQ/.github/blob/main/CONTRIBUTING.md) | 如何为任意项目做贡献 |

---

### 我们如何构建

| 原则 | 实践 |
|------|------|
| **先做再说** | 先出能跑的代码，再写提案。一个跑起来的原型胜过一份完美的规范。 |
| **大声发布** | 每次 merge、每个 release note、每位贡献者都有信号。发布应该像赢了一样。 |
| **默认开放** | 代码、路线图、决策、失败的实验——能开放的全部开放。 |

---

### 加入构建

这是社区项目，没有门槛。浏览 repo、开 PR、或者启动新的东西。

有问题请在相关 repo 开 issue，或在 [Discussion](https://github.com/orgs/effectorHQ/discussions) 中发起讨论。

---

<sub>每一个 effector 都在扩展边界。© 2026 effectorHQ Contributors</sub>

## License

This project is currently licensed under the [Apache License, Version 2.0](../LICENSE.md) 。
