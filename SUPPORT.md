# Getting Support

Different questions belong in different places. Picking the right channel gets you a faster answer.

## "How do I…?" / general questions

Use [**Discussions**](https://github.com/CommitBrief/commitbrief/discussions) on the CLI repository — it is the shared Q&A space for every CommitBrief project. If your question is about another repository and does not fit there, open an issue in that repository with the prefix `question:` in the title.

Examples:
- "How do I switch providers per repository?"
- "Does CommitBrief work with private GitLab repos?"
- "Best `COMMITBRIEF.md` patterns for a Rust project?"

## Bug reports

Use the **bug report** issue template in the affected repository. Include:

- The exact command you ran.
- What you expected vs. what happened.
- OS, architecture, CommitBrief version (`commitbrief --version`).
- Relevant config (redact API keys before pasting).

## Feature requests and proposals

Use the **feature request** issue template, or open a Discussion if the idea is broad and needs scoping first.

Substantive proposals are most useful when they describe:

1. **Motivation** — what is hard or impossible today.
2. **Proposal** — how it could work, even if rough.
3. **Alternatives** — other ways the same problem could be solved.

## Security vulnerabilities

Do **not** open a public issue. Report privately through GitHub's private vulnerability reporting as described in [SECURITY.md](SECURITY.md); email **info@muhammetsafak.com** only if you cannot use GitHub.

## Direct contact

For anything that does not fit the above — commercial use, integrations, sponsorship questions, anything off-channel — email **info@muhammetsafak.com**. Please keep public technical questions in public channels so others can benefit from the answer.

## What we cannot help with

- Account or billing questions for third-party AI providers (Anthropic, OpenAI, Google, DeepSeek, Mistral, Cohere, Ollama) or for the CLIs CommitBrief can drive (Claude Code, Gemini CLI, Codex CLI). Contact them directly.
- Generic Go / git questions unrelated to CommitBrief.
- "Please review my project's code" requests outside the documented `commitbrief` workflow.

## Response times

This is a maintainer-driven open source project. We respond as we can:

- **Security reports:** see [SECURITY.md](SECURITY.md) for target windows.
- **Bug reports with reproduction:** usually within a week.
- **Feature requests and Discussions:** when we have time and energy.
- **Pull requests:** depends on size and reviewability. Smaller, well-scoped PRs land faster.

If you have not heard back in two weeks and the issue is real, a polite bump on the thread is welcome.
