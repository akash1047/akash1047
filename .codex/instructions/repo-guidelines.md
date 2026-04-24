---
id: repo-guidelines-mirror
title: Repository Contribution Rules (Codex Mirror)
source_files:
  - AGENTS.md
audience: ai-agent
last_synced: 2026-04-24
sync_mode: manual
tags:
  - contribution
  - markdown
  - workflow
---

# Repository Contribution Rules (Codex Mirror)

## Intent

Mirror repository contribution guidance in a compact AI-first structure.

## Rules

- Treat this repository as documentation-first.
- Primary editable areas: `README.md`, `context/`, `resume/`.
- Update order for role-content changes:
  1. `context/master-profile.md`
  2. `context/role-playbooks/`
  3. `resume/`
- Use concise Markdown and measurable statements.
- Keep all content public-safe.

## Validation

- Check evidence structure with `rg "Evidence ID|Role Fit" context/`.
- Review scoped diffs using `git diff -- README.md context/ resume/`.
- Verify timeline and title consistency across profile, context, and resumes.

## Output Quality

- Preserve naming patterns for role files.
- Keep commit messages imperative and scoped.
- Include change reason and consistency/privacy checks in PR notes.

