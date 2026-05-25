# CommitBrief — Organization Defaults

This repository hosts the default community health files and templates that GitHub applies across every repository in the [CommitBrief](https://github.com/CommitBrief) organization.

It is not a code repository. Nothing here is shipped to production.

## What lives here

| Path | Purpose |
|---|---|
| `profile/README.md` | Public organization profile shown on `github.com/CommitBrief`. |
| `SECURITY.md` | Vulnerability reporting policy for all org repositories. |
| `CODE_OF_CONDUCT.md` | Behavioral expectations for org members and contributors. |
| `CONTRIBUTING.md` | Contribution workflow. CommitBrief is a closed-source project; contributions are by invitation. |
| `SUPPORT.md` | How to get help and which channel to use. |
| `PULL_REQUEST_TEMPLATE.md` | Default PR template applied to every repository. |
| `ISSUE_TEMPLATE/` | Default issue forms (bug report, feature request) and configuration. |

## How GitHub uses these files

GitHub falls back to this repository when a given file is not present in the repository where the action originates. Anything defined inside an individual repository takes precedence over the version here.

Order of precedence for community health files (highest first):

1. The repository itself (e.g. `repos/commitbrief-api/.github/`)
2. This organization-level `.github` repository
3. The user's personal `.github` repository (not used by this org)

## Overriding defaults per repository

Drop a file with the same name under a repository's own `.github/` directory to override the default. For example, a repository can define its own `PULL_REQUEST_TEMPLATE.md` to capture domain-specific checks beyond the org default.

## Visibility

This repository is public so the organization profile page renders for everyone. The rest of the CommitBrief organization is private and stays that way.
