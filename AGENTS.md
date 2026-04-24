# Repository Guidelines

## Project Structure & Module Organization

This repository is a documentation-first GitHub profile project.

- `README.md`: Public profile landing page.
- `context/`: Canonical career knowledge base used to generate role-specific content.
- `context/master-profile.md`: Source-of-truth timeline, skills, and evidence blocks.
- `context/role-playbooks/`: Role positioning (`frontend`, `backend`, `fullstack`, `devops`, `ai`).
- `context/tailoring-prompts.md`: Prompt templates for resume generation.
- `resume/`: Tailored resume drafts (`frontend.md`, `backend.md`, `fullstack.md`, `devops.md`).
- `.codex/instructions/`: AI-readable instruction mirrors for Codex workflows.

Keep role updates consistent: update `context/master-profile.md` first, then playbooks, then `resume/`.

## AI Instruction Mirrors

Use [`.codex/instructions/index.md`](/home/akash/iam/akash1047/.codex/instructions/index.md) as the machine entrypoint.  
Human-facing docs remain canonical; mirror files are synchronization aids.

## Build, Test, and Development Commands

No build pipeline exists; changes are content-based and validated with lightweight checks.

- `rg --files`: List tracked content quickly.
- `rg "Evidence ID|Role Fit" context/`: Verify evidence schema usage.
- `git diff -- README.md context/ resume/`: Review only profile-related edits before commit.
- `git diff -- AGENTS.md .codex/ context/`: Review instruction mirror sync.
- `git log --oneline -n 10`: Check recent commit style and scope.

## Coding Style & Naming Conventions

- Use Markdown with short sections, clear headings, and scannable bullets.
- Keep language factual, measurable, and public-safe.
- Use lowercase kebab-case for new file names (example: `site-reliability.md`).
- Preserve existing naming patterns for role files (`frontend.md`, `backend.md`, etc.).

## Testing Guidelines

Testing is editorial consistency rather than unit tests.

- Confirm dates/titles match across `README.md`, `context/master-profile.md`, and `resume/*.md`.
- Ensure each strong resume bullet maps to an evidence block in `context/`.
- Validate privacy: no phone number, private identifiers, or sensitive internal details.
- Run a quick preview in your Markdown viewer to check formatting.

## Commit & Pull Request Guidelines

Use concise, imperative commit subjects, aligned with current history:

- `Add tailored resumes for frontend backend fullstack and devops`
- `Add resume tailoring context knowledge base`
- `Create GitHub profile README`

PRs should include:

- What changed (files/sections).
- Why it changed (new role, updated outcomes, targeting a JD).
- Consistency check completed (timeline, evidence mapping, privacy).
