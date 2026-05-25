# Contributing to CommitBrief

CommitBrief is a closed-source project. The repositories under this organization are not open for unsolicited external contributions, and most of them are private.

This document exists for two reasons:

1. To set expectations for invited collaborators and org members who do work inside these repositories.
2. To make it clear how anyone outside the organization can still report bugs, suggest improvements, or flag editorial issues with content we publish.

## If you are not an org member

You are welcome to:

- Open an issue on a public repository using the issue templates.
- Email feedback or content corrections to **commitbrief@muhammetsafak.com.tr**.
- Report a security finding through the process in [SECURITY.md](./SECURITY.md).

Please do not open pull requests against private repositories without prior discussion. We may not be able to accept or even review external code changes at this stage.

## If you are an org member or invited collaborator

The rest of this document is for you.

### Workflow

- Work on a feature branch off `main`. Never push directly to `main`.
- Open a pull request when the work is ready for review. Draft PRs are encouraged for in-progress work that needs early feedback.
- At least one approving review is required before merge. The repository's CI must be green.
- Prefer squash merges. The squash commit message should follow the same convention as individual commits.
- Do not force-push to shared branches (`main`, release branches). Force-pushing your own feature branch is fine until review starts.

### Branch naming

Use `<type>/<short-description>`, kebab-cased:

```
feat/source-clustering-engine
fix/gatekeeper-prompt-timeout
chore/bump-dramatiq-1.17
docs/adr-008-vector-index-strategy
refactor/llm-provider-adapter
```

Allowed types: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`, `perf`, `build`, `ci`.

### Commit messages

We follow [Conventional Commits](https://www.conventionalcommits.org/) so commit history stays parseable for changelogs and release tooling.

```
<type>(<scope>): <subject>

<body>

<footer>
```

Examples:

```
feat(ingestion): add Hacker News upvote threshold filter
fix(scoring): correct CVSS normalization for Tier 0 sources
docs(adr): record decision to use pgvector for V1
```

The body is optional. If the change is non-trivial, explain *why* in the body, not what — the diff already shows what.

### Pull requests

- Fill out the PR template in full. Do not delete sections; mark them N/A if they do not apply.
- Link the related issue or design doc.
- Call out any breaking changes, schema migrations, prompt version bumps, or security-relevant changes explicitly.
- Add or update tests for behavior changes.
- Update documentation in the same PR when the change affects how a system is operated.

### Reviewing

- Review for correctness, security, and operational impact first; style preferences second.
- Use suggestions rather than re-writing code when possible.
- A review with only blocking comments and no acknowledgement of the work is rude. Acknowledge what was done well, then ask for changes.

### Local development

Each repository documents its own setup in its `README.md`. There is no shared scaffold across the polyrepo at this time.

### Questions

For questions about how to contribute, the architecture, or whether something fits the roadmap, reach out internally rather than posting public issues that may leak roadmap information.
