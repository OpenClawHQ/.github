# Contributing to OpenClawHQ

Thanks for showing up. This guide applies to all repositories under the OpenClawHQ organization.

## Principles

Before anything else — our three operating principles:

1. **Build First.** A working prototype beats a perfect proposal. Ship rough, iterate in the open.
2. **Ship Loud.** Don't build in silence. Share early. A typo fix and a core connector carry equal weight.
3. **Open by Default.** Code, roadmap, decisions. If it can be open, it is.

## How to contribute

### Found a bug or have an idea?

Open an issue. Use the templates provided. Be specific — include steps to reproduce for bugs, or a clear description of the use case for feature requests.

### Want to fix or build something?

1. **Fork** the repository.
2. **Create a branch** from `main`. Name it descriptively: `feat/add-slack-connector`, `fix/auth-timeout`, `docs/update-readme`.
3. **Make your changes.** Follow the existing code style. Write tests if the repo has a test suite.
4. **Commit** using our [Commit Convention](COMMIT_CONVENTION.md).
5. **Open a Pull Request** against `main`. Fill out the PR template. Link related issues.
6. **Respond to review.** We aim to review PRs within 48 hours.

### Not sure where to start?

Look for issues tagged `good first issue` or `help wanted`. These are specifically marked for new contributors.

## Code style

Each repo may have its own style guide or linter config. When in doubt:

- Follow the conventions you see in the existing code.
- Consistency within a file > personal preference.
- If the repo has a formatter (Black, Prettier, etc.), run it before committing.

## Commit messages

We follow a lightweight convention based on [Conventional Commits](https://www.conventionalcommits.org/). See [COMMIT_CONVENTION.md](COMMIT_CONVENTION.md) for the full spec.

Short version:

```
feat: add Slack connector
fix: resolve auth timeout on retry
docs: update plugin-template README
```

## Pull requests

- Keep PRs focused. One logical change per PR.
- Write a clear description of **what** changed and **why**.
- Include screenshots or recordings for UI changes.
- If the PR is work-in-progress, open it as a **Draft PR** and mark it clearly.

## Issues and discussions

- **Issues** are for actionable items: bugs, feature requests, specific tasks.
- **Discussions** (when enabled) are for open-ended questions, ideas, and general conversation.
- Be respectful. We're all building in the same direction.

## Licensing

Unless stated otherwise, contributions to OpenClawHQ repos are licensed under the same license as the repo you're contributing to. By submitting a PR, you agree that your contribution will be licensed accordingly.

## Recognition

Every contribution matters. We maintain contributor lists and credit authors in changelogs. If you contribute, you're part of the build.

---

Questions? Open an issue or start a discussion. We're glad you're here.

---

<!-- TEST: This block is for testing the labeler/size/typo CI bot. Do not merge. -->
## [TEST] Bot test block (ignore)

This paragrah has intentional errrors: teh word "occurred" is misspelled as "occured", and "separate" as "seperate". The rest of the sentence is correct: we run Security Analysis, Simple checks, Typo, and Build workflows. Size labels (XS/S/M/L/XL) are applied automatically. You can safely close this PR without merging.
