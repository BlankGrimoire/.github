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

1. **No real website domains** anywhere (code, tests, comments, commit messages, docs). Use `example.org` / `example.com` only.
2. **Themes, not websites.** No site-specific scrapers, no lists of sites, no adapters named after sites.
3. **Synthetic fixtures only.** Hand-written Lorem ipsum and placeholder images. Never copy HTML, text, or images from real sites.
4. **No circumvention.** No bypass of authentication, paywalls, DRM, or access controls. Anti-bot challenges are completed by the user in a **visible** WKWebView, never a hidden one.
5. **Attribution preserved.** Site name, logo, credits, and the "Open on site" button. Credit pages are never filtered.
6. **No marketing vocabulary.** The words manga, manhwa, and scanlation must not appear in descriptions, topics, or README marketing. Domain type names (e.g. `MangaSummary`) are acceptable in code.
7. **Never commit secrets.** The Ed25519 private key lives only in GitHub environment secrets.
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
