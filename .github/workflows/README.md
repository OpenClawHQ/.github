# Workflows

Reusable workflows in this directory are for use by repos in the org.

## Simple tests (Security / Simple checks / Typo / Build)

- **simple-tests.yml** — Runs on push/PR to `main`: Security Analysis, Simple checks, Typo, Build.
- Other repos can add the same **simple-tests.yml** in their `.github/workflows/` to call these reusable workflows.

## Reusable workflows

| File | Purpose |
|------|---------|
| **security-analysis.yml** | Runs `npm audit` when `package.json` exists; optionally `pip-audit` for Python deps. |
| **simple-checks.yml** | Checks for committed secrets in .env; validates YAML under `.github`. |
| **typo.yml** | Runs [crate-ci/typos](https://github.com/crate-ci/typos) for spell/typo checks. |
| **build.yml** | With `package.json`: `npm ci` + `npm test`; Python-only: `pip install` + `pytest`. Job timeout 5 min. |
| **reusable-skill-lint.yml** | Validates SKILL.md; for skill repos to call. |

## Dependabot

**.github/dependabot.yml** at repo root is configured for weekly GitHub Actions upgrade PRs (no CI time). Repos with `package.json` have their own dependabot (npm + github-actions).

## Repos using simple-tests

- This repo (.github)
- skill-lint
- skill-lint-action
- plugin-template
- cookbook
- linear-skill

Copy **simple-tests.yml** into a repo’s `.github/workflows/` to enable the same checks.

## Labels and auto-labeling (Labeler)

- **docs/LABELS.md** — Label taxonomy (type / area / priority / source / **size**), colors, and descriptions; create in each repo via Settings → Labels.
- **.github/labeler.yml** — Rules to auto-apply labels from PR file paths (e.g. `.md` → `documentation`, `.github/**` → `area: meta`).
- **.github/workflows/labeler.yml** — Runs on PR open/sync:
  - **label-by-path**: applies type/area from changed paths.
  - **label-size**: adds one of `size: XS` / `size: S` / `size: M` / `size: L` / `size: XL` from additions + deletions (see LABELS.md for thresholds).
  - **label-bot**: adds `bot` (and `dependencies` for Dependabot) for bot-authored PRs.

Create the five size labels in the repo so the size job can apply them. Copy **labeler.yml** and **workflows/labeler.yml** into a repo to reuse.
