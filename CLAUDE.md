# CLAUDE.md

This is a documentation-first GitHub profile repository — no build, no app code. Content changes only.

## Project structure

- `README.md`: Public profile landing page.
- `context/`: Canonical career knowledge base used to generate role-specific content.
- `context/master-profile.md`: Source-of-truth timeline, skills, and evidence blocks.
- `context/role-playbooks/`: Role positioning (`frontend`, `backend`, `fullstack`, `devops`, `ai`).
- `context/tailoring-prompts.md`: Prompt templates for resume generation.
- `resume/`: Tailored resume drafts (`frontend.md`, `backend.md`, `fullstack.md`, `devops.md`).

## Non-negotiable rules

- **Update order for role content**: `context/master-profile.md` → `context/role-playbooks/` → `resume/`. Never edit a resume without checking it still traces back to the master profile.
- **No invented claims or metrics.** Every strong resume bullet must map to an existing Evidence ID in `context/`. Add new outcomes as new evidence entries — don't rewrite history.
- **Public-safe only.** No phone numbers, private identifiers, or sensitive internal business details in any tracked file.
- **Consistency check before finishing**: dates, titles, and company names must match exactly across `README.md`, `context/master-profile.md`, and `resume/*.md`.

## Coding style

- Markdown with short sections, clear headings, scannable bullets.
- Factual, measurable, public-safe language.
- Lowercase kebab-case for new file names (example: `site-reliability.md`).
- Preserve existing naming patterns for role files.

## Verification commands

- `rg --files` — list tracked content quickly.
- `rg "Evidence ID|Role Fit" context/` — confirm evidence schema usage.
- `git diff -- README.md context/ resume/` — scope review to profile content.

## Commit & PR conventions

Concise, imperative commit subjects, e.g. `Add tailored resume for backend`.

PRs should note: what changed, why (new role / updated outcome / targeting a JD), and confirmation that the consistency check (timeline, evidence mapping, privacy) was done.
