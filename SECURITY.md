# Security Policy

CommitBrief processes vulnerability data, runs an LLM-driven content pipeline, and publishes to public channels. We take security seriously and welcome reports from anyone who finds an issue.

## Scope

This policy covers every repository owned by the [CommitBrief](https://github.com/CommitBrief) GitHub organization, including the data pipeline, APIs, prompts, infrastructure-as-code, and the public-facing distribution surface.

Out of scope:

- Third-party platforms we publish to (X, LinkedIn, Substack) — report directly to the platform
- LLM provider infrastructure (OpenAI, Anthropic, Google) — report directly to the provider
- Issues already publicly disclosed without prior coordination

## How to report a vulnerability

**Do not open a public GitHub issue for a security report.**

Use one of the following private channels:

1. **GitHub Security Advisory (preferred)** — open a private advisory on the affected repository via the *Security* tab. This keeps the report scoped to the right codebase and gives you a private discussion thread.
2. **Email** — send a report to **commitbrief@muhammetsafak.com.tr** with the subject prefix `[SECURITY]`.

Please include, at minimum:

- A description of the issue and its impact
- The affected repository, service, or endpoint
- Reproduction steps or a proof of concept
- Any logs, payloads, or screenshots that help us confirm the issue
- Your preferred contact and whether you want public credit on disclosure

If you are reporting a finding that is time-sensitive (active exploitation, exposed credentials, data leakage), say so in the subject line.

## What to expect

| Stage | Target |
|---|---|
| Initial acknowledgement | within 3 business days |
| Triage and severity assessment | within 7 business days |
| Status update cadence during remediation | at least every 14 days |
| Coordinated disclosure window | up to 90 days from confirmed report, negotiable for complex issues |

We will keep you informed during triage, validate the issue, work on a fix, and coordinate disclosure timing with you. We do not currently operate a paid bug bounty program, but we are happy to publicly credit reporters who request it.

## Safe harbor

We will not pursue legal action against researchers who:

- Make a good-faith effort to comply with this policy
- Avoid privacy violations, service disruption, and destruction of data
- Do not access more data than is necessary to demonstrate the vulnerability
- Give us a reasonable window to remediate before public disclosure

If in doubt, contact us first.

## Out-of-band concerns

If you believe a published CommitBrief story contains a factual error or misrepresents a security advisory, that is an editorial issue rather than a vulnerability. Please open a regular issue on the relevant repository or email us at the address above without the `[SECURITY]` prefix.
