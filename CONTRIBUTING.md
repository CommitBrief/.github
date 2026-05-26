# Contributing to CommitBrief

Thanks for thinking about contributing. This document is the org-wide default; individual repositories may override it with their own `CONTRIBUTING.md` that adds project-specific guidance (build commands, repo layout, etc.).

## TL;DR

1. Open an **issue first** for anything non-trivial. We would rather discuss before you spend time.
2. Read the [Code of Conduct](CODE_OF_CONDUCT.md).
3. Fork, branch, code, push, open a pull request.
4. Be patient with reviews — this is a side-project for the maintainers.

## How we accept contributions

CommitBrief uses the **inbound = outbound** licensing model. By opening a pull request you agree that your contribution is licensed to the project under the **GPL-3.0-or-later** license that governs the repository. There is no separate Contributor License Agreement (CLA) and no Developer Certificate of Origin (DCO) sign-off is required.

If your employer or another party may claim rights over your contribution, please confirm with them before submitting.

## Issues

Before opening an issue:

- Search existing **open and closed** issues — you may not be the first to hit it.
- For bugs, prefer the **bug report** template and fill in every field. Reproduction steps with the exact command, OS, and version save us hours.
- For features, prefer the **feature request** template and describe the motivation first, the proposal second.
- For "how do I…" or "is this supported?" questions, use **Discussions** instead of Issues.

## Pull requests

- Keep PRs **focused**. One logical change per PR. Refactors that touch many files should be split into preparatory PRs and the substantive change.
- Write the PR description with a **summary** and a **test plan**. The PR template captures both.
- Reference related issues with `Fixes #N` or `Refs #N`.
- Run `make lint test` locally before pushing. CI will run the same checks plus a build matrix.
- **Commit messages** follow [Conventional Commits](https://www.conventionalcommits.org/) on the default branch. Examples:
  - `feat(provider): add Mistral support`
  - `fix(cache): handle TTL boundary correctly`
  - `docs: clarify --staged behavior`

## Coding style

- **Go:** the codebase uses `gofmt`, `goimports`, and `golangci-lint` with the project's `.golangci.yml`. CI rejects unformatted or lint-failing PRs.
- **Comments:** explain *why*, not *what*. Code should be readable on its own.
- **Tests:** add tests for every behavior change. Aim for the smallest test that demonstrates the issue.
- **Public-facing strings** in the CLI go through `internal/i18n`. Never hard-code user-visible text; use a key with entries in both `messages.en.yml` and `messages.tr.yml`.

## Security issues

Do **not** open a public issue for security reports. See [SECURITY.md](SECURITY.md) for the private reporting channel.

## Project-specific contributing guides

Some repositories add their own `CONTRIBUTING.md` with extra detail (build commands, architecture overview, integration test setup). When present, that project-level file extends this one — both apply.

## Questions

Open a **Discussion** in the relevant repository, or email **info@muhammetsafak.com.tr** for anything that needs to be off-channel.

Thank you for helping us improve CommitBrief.
