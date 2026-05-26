# Security Policy

This document applies to **all repositories under the [CommitBrief](https://github.com/CommitBrief) organization**. Individual repositories may publish a project-specific `SECURITY.md` that supplements this document.

## Reporting a vulnerability

**Please do not open a public issue for security reports.**

Send vulnerability reports privately to:

**info@muhammetsafak.com.tr**

If GitHub Security Advisories are enabled on the affected repository, you may also use the [private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability) feature.

Include in your report:

- A clear description of the issue and its potential impact.
- Steps to reproduce, including a minimal proof-of-concept if possible.
- Affected version(s), operating system, and any relevant configuration.
- Your assessment of severity (low / medium / high / critical) — feel free to disagree with our final triage.

## What to expect

| Stage | Target window |
|-------|---------------|
| Acknowledgment of report | within 5 business days |
| Initial triage and severity assessment | within 10 business days |
| Fix or mitigation timeline | shared once triage completes |
| Public advisory (after fix) | coordinated with reporter |

This is a maintainer-driven open source project, not a commercial product with an SLA. We will make a genuine best effort but cannot promise enterprise-grade response times.

## Disclosure

We follow **coordinated disclosure**:

1. You report privately.
2. We triage and develop a fix.
3. We release the fix in a patched version.
4. We publish a security advisory crediting you (unless you prefer to remain anonymous), describing the issue, and noting the affected versions and the fix.

We will not publish details before a fix is available, and we ask you to do the same.

## Supported versions

Security patches are issued for the **latest released minor version** of each project. Once a project reaches v1.0, the policy will be revisited; until then, expect rolling updates on the current release line.

## Acknowledgments

We are happy to credit security reporters in release notes and advisories. Let us know your preferred name and (optionally) a contact URL.

## Out of scope

The following are generally **not** considered security issues for the purposes of this policy:

- Vulnerabilities in third-party AI provider APIs (report to the provider directly).
- Issues that require physical access to a user's already-compromised machine.
- API key leakage caused by the user committing their own `.commitbrief/config.yml` (we provide multiple safeguards; the residual risk is a user-environment concern).
- Theoretical timing or side-channel attacks without a demonstrated practical impact.

Edge cases will be evaluated on a case-by-case basis. When in doubt, send the report and we will decide together.
