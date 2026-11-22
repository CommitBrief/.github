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

GitHub uses a file from this repository only when the target repository does not have its own. For a given file, GitHub looks in the target repository's `.github/` directory, its root, and its `docs/` directory; if none of them has the file, it falls back to the copy here.

A few details worth knowing:

- Issue templates are all-or-nothing: if a repository has its own `.github/ISSUE_TEMPLATE/` directory, none of the templates here (including `config.yml`) apply to it.
- `LICENSE` is never inherited; every repository carries its own.
- This repository must stay **public**; GitHub ignores defaults from a private `.github` repository.

In practice: **add a file to a specific repository to override the default here**.

## License

The content of this repository is released under the **GPL-3.0-or-later** license, matching the rest of the CommitBrief organization.

## Maintainers

If you find an outdated link, typo, or unclear policy in any of these files, please open an issue or a pull request.
