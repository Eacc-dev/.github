# CLAUDE.md

## Repository Overview

This is the **GitHub organization-level `.github` repository** for the **Eacc-dev** organization. It serves as the public-facing profile and organization-wide configuration hub for the CodeSama project — an AI-powered code review and bug fix assistant.

## Repository Structure

```
.github/
├── CLAUDE.md              # This file — guidance for AI assistants
├── README.md              # Legacy root README (Probot-based "code-review-master" app)
├── profile/
│   └── README.md          # Organization profile README displayed on GitHub org page
└── .git/
```

**Total files:** 2 Markdown documents (plus this file).

### Key Files

- **`profile/README.md`** — The authoritative organization profile. Describes CodeSama's features (smart code reviews, async code generation, interactive Q&A, changelog generation) and links to documentation, support, and community resources. This is what visitors see on the GitHub organization page.
- **`README.md`** (root) — Legacy README for "code-review-master," a Probot-based GitHub App. Contains setup instructions (`npm install` / `npm start`) and Docker build steps. Predates the CodeSama branding.

### Content Note

The root `README.md` and `profile/README.md` describe different products/branding stages. The profile README (CodeSama) represents the current state; the root README (code-review-master) is historical.

## Development Conventions

### Branching

- Default branch: `master`
- Feature/task branches follow the pattern: `claude/<descriptor>-<session-id>`

### Commits

- Commit messages have been short and descriptive (e.g., "Update README.md")
- All historical commits are documentation-only changes

### Documentation Style

- Markdown with GitHub-flavored formatting
- Features organized with `###` subsections under `##` headings
- Bold text (`**...**`) used for feature names and key terms in lists
- Product references use the name **CodeSama** with the GitHub handle `@CodeSama-dev`

## What This Repository Does NOT Contain

This is a documentation-only repository. The following are **not present**:

- GitHub Actions workflows (no `workflows/` directory)
- Issue templates or PR templates
- CONTRIBUTING.md (referenced in root README but never created)
- CODE_OF_CONDUCT.md
- SECURITY.md
- FUNDING.yml
- LICENSE file (referenced but not present)
- Any source code, build scripts, or dependencies

## Guidelines for AI Assistants

1. **No build/test/lint steps exist** — this repo has no code to compile or test.
2. **Treat `profile/README.md` as the primary document** — it represents the current organization identity (CodeSama).
3. **The root `README.md` is legacy content** — changes to organization messaging should target `profile/README.md`.
4. **Keep changes minimal** — this is a small, documentation-focused repo. Avoid introducing unnecessary complexity.
5. **Preserve existing formatting conventions** — use the same Markdown heading hierarchy and bold/list patterns found in the existing files.
6. **Missing standard files** — if asked to add issue templates, PR templates, workflows, or policy documents, place them according to [GitHub's `.github` repository conventions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions).
