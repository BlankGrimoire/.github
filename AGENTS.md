# AGENTS.md

Instructions for AI coding agents working in this repository.
Human contributors: see `CONTRIBUTING.md` (if present) and the organization's `.github` repository.

## Repository Facts

| Key | Value |
|-----|-------|
| Repository | .github |
| Stack | Markdown community health files |
| License | n/a (inherits the organization defaults; ask the human if unclear) |
| Source header | None |
| Contact | blankgrimoire.dev@gmail.com |
| Copyright holder | BlankGrimoire contributors |

## Non-Negotiable Rules

1. **Flexible Endpoint Configuration.** Avoid hardcoding explicit real-world domains in code, tests, or documentation. Use configurable base URLs or generic identifiers (e.g., `SourceTypeA`, `TemplateB`) to abstract the underlying fan-site infrastructure.
2. **Generic Theme Adapters.** Scrapers and adapters must be designed around structural layout themes rather than being explicitly named after specific websites. Build them to support families of sites with similar architectures, keeping the actual target domains masked and dynamically injected.
3. **Abstracted Test Data.** Avoid bundling extensive real content from external platforms in the repository.
4. **Silent anti-bot resolution first.** Adapters should attempt to handle and bypass standard anti-bot challenges or captchas automatically and transparently in the background. Only if automated resolution fails or is technically unfeasible must the challenge be deferred to the user via a visible WKWebView.
5. **Attribution preserved.** Site name, logo, credits, and the "Open on site" button must remain intact. Credit pages are never filtered.
6. **No marketing vocabulary.** The words manga, manhwa, and scanlation must not appear in descriptions, topics, or README marketing. Domain type names (e.g. `MangaSummary`) are acceptable in code. Published adapter names and descriptions are validated at build time.
7. **Never commit secrets.** The Ed25519 private key lives only in GitHub environment secrets. Local keys and certificates are gitignored.
8. **Never commit personal emails.** The only allowed email is blankgrimoire.dev@gmail.com.

## Git Rules

- Never `git push`, never force push, never create remote resources, never publish packages.
- Conventional Commits only: `feat`, `fix`, `perf`, `refactor`, `docs`, `chore`, `ci`, `test`, `revert`; use `!` for breaking changes.
- Branches: `feat/<topic>`, `fix/<topic>`, `docs/<topic>`.
- Squash merge; the PR title is the commit message and drives semantic-release.
- Never edit `CHANGELOG.md` by hand. Never create release tags manually.

## Code Style

English, neutral wording, no marketing vocabulary (Rule 6), contact email only.

## Commands

| Task | Command |
|------|---------|
| Check required files exist | `ls SECURITY.md CODE_OF_CONDUCT.md PULL_REQUEST_TEMPLATE.md ISSUE_TEMPLATE profile/README.md` |
| Hygiene scans | See handout 00, §3.2 |

## Before Every Commit

- [ ] All commands in the table above pass.
- [ ] Every new source file has the license header.
- [ ] Domain, vocabulary, secrets, and email scans are clean.
- [ ] No new dependencies without human approval.

## Ask a Human Before

- Adding dependencies not listed in the handouts.
- Changing the adapter contract after SDK-1 approval.
- Anything touching remotes, repository settings, or secrets.
- App icon or branding, distribution or code signing, and license questions.
