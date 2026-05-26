# `.github` — Organization defaults

This repository holds the community health files and templates that apply to **every repository under the [CommitBrief](https://github.com/CommitBrief) organization** by default.

> If a file in this repository conflicts with a file at the same path in a specific repository, **the file in that repository wins**. This repository provides defaults; individual repositories can override.

## What is here

| File / directory | Purpose |
|------------------|---------|
| [`profile/README.md`](profile/README.md) | The organization profile page shown at <https://github.com/CommitBrief>. |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Code of conduct (Contributor Covenant v2.1) applied across all CommitBrief projects. |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Default contribution guidelines: licensing, PR conventions, coding style. |
| [`SECURITY.md`](SECURITY.md) | How to report a vulnerability privately. |
| [`SUPPORT.md`](SUPPORT.md) | Where to ask questions, report bugs, and request features. |
| [`FUNDING.yml`](FUNDING.yml) | GitHub Sponsors configuration. |
| [`ISSUE_TEMPLATE/`](ISSUE_TEMPLATE/) | Default issue templates (bug report, feature request) and the chooser config. |
| [`PULL_REQUEST_TEMPLATE.md`](PULL_REQUEST_TEMPLATE.md) | Default pull request template. |

## How overrides work

GitHub looks for a file in this order when a repository event needs one:

1. `repo/.github/<file>` — repository-specific override.
2. `repo/<file>` — at the repository root.
3. `org/.github/.github/<file>` — this repository (with `.github/` prefix for templates).
4. `org/.github/<file>` — this repository (for `CONTRIBUTING.md`, `SECURITY.md`, etc.).

In practice: **add a file to a specific repository to override the default here**.

## License

The content of this repository is released under the **GPL-3.0-or-later** license, matching the rest of the CommitBrief organization.

## Maintainers

If you find an outdated link, typo, or unclear policy in any of these files, please open an issue or a pull request.
