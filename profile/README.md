<!--
  Bu dosya, GitHub'da https://github.com/CommitBrief sayfasında görünür.
  Marketing odaklı: pitch + neden + ürünler + nasıl başlanır.
-->

# CommitBrief

> **LLM-powered code review for your local commits — before another human sees them.**

CommitBrief is a developer-first toolchain that brings AI code review into the terminal, right next to `git`. No web UI, no SaaS dashboard, no telemetry — just a faster feedback loop on the code you are about to commit.

[![Latest release](https://img.shields.io/github/v/release/CommitBrief/commitbrief?sort=semver&label=latest&color=2ea043)](https://github.com/CommitBrief/commitbrief/releases/latest) [![License](https://img.shields.io/badge/license-GPL--3.0--or--later-blue)](https://github.com/CommitBrief/commitbrief/blob/main/LICENSE) [![Platforms](https://img.shields.io/badge/platforms-Linux%20%7C%20macOS%20%7C%20Windows-informational)](https://github.com/CommitBrief/commitbrief/releases/latest)

<!-- Duyuru bloğu: her yeni release'de sürüm + headline özelliği güncelle. -->
> [!NOTE]
> 🎉 **`v1.1.0` is out.** CommitBrief is now **stable** (strict semver since `v1.0.0`) and ships **`commitbrief remote pr <ID>`** — review a GitHub pull request straight from your terminal: each finding is posted as an inline review comment, plus an approve / comment / request-changes verdict. Install via Homebrew, Scoop, or `go install`. → [Release notes](https://github.com/CommitBrief/commitbrief/releases/latest)

---

## Why?

Every modern engineer ships code under two opposing pressures: review thoroughness and review latency. Today the options are:

- **Re-read your own diff** — slow, easy to miss issues, inconsistent.
- **Ask a colleague** — high-quality, but a costly synchronous round-trip.
- **Paste into a chat UI** — friction, no project rules, no caching, no git context.

CommitBrief fills the gap: a five-second AI-assisted pre-check on the diff in front of you, using rules **you defined**, run against the AI provider **you chose** (including local-only Ollama).

---

## Get started

```sh
brew install commitbrief        # macOS + Linux
# or
go install github.com/CommitBrief/commitbrief@latest

commitbrief setup               # one-time interactive provider + API key setup
commitbrief                     # review your currently staged changes
```

Want a fully local, privacy-first setup? Point CommitBrief at Ollama and your favorite local model — no data leaves your machine.

---

## Products

| Project | Description | Status |
|---------|-------------|--------|
| [**commitbrief**](https://github.com/CommitBrief/commitbrief) | The CLI: review `--staged` / `--unstaged`, any `git diff` range, or a GitHub PR (`remote pr`). Structured findings in your terminal, in your language. | **Stable — v1.1.0** |

Companion tools (planned):
- A GitHub Action that runs CommitBrief in CI on pull requests.
- A VS Code extension that wraps the CLI for in-editor reviews.

---

## Principles

- **Privacy-first.** No telemetry, no remote config, no shared state. Your code stays where you put it.
- **Provider-agnostic.** Anthropic, OpenAI, Google Gemini, and local Ollama supported out of the box. No vendor lock-in.
- **Developer-controlled.** You define the review rules in plain Markdown in your repo. CommitBrief reads them as the system prompt — no DSL to learn.
- **Terminal-native.** Streaming output, color, glamour-rendered Markdown. JSON when you need to script around it.
- **Open source.** All projects under **GPL-3.0**.

---

## Contact

- **General questions:** open a discussion on the relevant repo.
- **Bug reports:** open an issue with the bug-report template.
- **Security:** see each repo's `SECURITY.md`, or email **info@muhammetsafak.com.tr**.

---

> Free your commits from the "looks good to me" reflex. Run `commitbrief` and let the diff speak.
