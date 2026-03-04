# OpenClawHQ Label Conventions

Repos can create the following labels under **Settings → Labels** for categorization and auto-labeling. The Labeler action applies labels to PRs based on changed file paths.

---

## 1. Type — Kind of work

| Label | Color | Description |
|-------|--------|--------------|
| `bug` | `#d73a4a` | Something is broken; needs a fix |
| `enhancement` | `#a2eeef` | New feature or improvement |
| `documentation` | `#0075ca` | Documentation-only changes |
| `refactor` | `#fef2c0` | Refactor; neither bug fix nor new feature |
| `chore` | `#f9d0c4` | Build, CI, tooling, config |
| `dependencies` | `#0366d6` | Dependency updates (e.g. Dependabot) |
| `security` | `#b60205` | Security-related |

---

## 2. Area — Scope

| Label | Color | Description |
|-------|--------|--------------|
| `area: skill` | `#c5def5` | SKILL.md, skills directory |
| `area: extension` | `#c5def5` | Extension / plugin logic |
| `area: cli` | `#c5def5` | CLI commands and interaction |
| `area: action` | `#c5def5` | GitHub Action |
| `area: docs` | `#c5def5` | Docs site, guides, reference |
| `area: website` | `#c5def5` | Org website |
| `area: infra` | `#c5def5` | CI, workflows, config |
| `area: meta` | `#d4c5f9` | .github, org defaults |

---

## 3. Priority — Optional; often for issues

| Label | Color | Description |
|-------|--------|--------------|
| `priority: critical` | `#b60205` | Urgent |
| `priority: high` | `#d93f0b` | High |
| `priority: medium` | `#fbca04` | Medium |
| `priority: low` | `#0e8a16` | Low |

---

## 4. Source — Human vs bot

| Label | Color | Description |
|-------|--------|--------------|
| `bot` | `#ededed` | Opened by automation (e.g. Dependabot) |

---

## 5. Size — PR change size (auto-applied)

| Label | Color | Description (total lines: additions + deletions) |
|-------|--------|---------------------------------------------------|
| `size: XS` | `#0e8a16` | ≤ 10 lines |
| `size: S`  | `#0e8a16` | 11–30 lines |
| `size: M`  | `#fbca04` | 31–100 lines |
| `size: L`  | `#d93f0b` | 101–500 lines |
| `size: XL` | `#b60205` | > 500 lines |

The Labeler workflow computes the PR diff and adds exactly one of these labels. Create all five in **Settings → Labels** for the job to succeed.

---

## 6. Auto-labeling (Labeler)

1. **By path**: PRs get type/area labels from changed file paths; rules live in **.github/labeler.yml**.
2. **Bot PRs**: PRs opened by Dependabot or github-actions[bot] get `bot` (and `dependencies` for dependency updates).

Copy **.github/labeler.yml** and **.github/workflows/labeler.yml** into a repo to reuse the same rules.

---

## 7. Creating these labels in a repo

- **Option A**: In each repo, go to **Settings → Labels** and create them from the tables above.
- **Option B**: Use the GitHub API or an action such as [github-label-sync](https://github.com/marketplace/actions/github-label-sync) to create/sync labels from a YAML file (requires a token).
