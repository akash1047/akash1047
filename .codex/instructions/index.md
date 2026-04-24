---
id: codex-instruction-index
title: Codex Instruction Index
source_files:
  - AGENTS.md
  - context/README.md
  - context/maintenance-guide.md
  - context/tailoring-prompts.md
audience: ai-agent
last_synced: 2026-04-24
sync_mode: manual
tags:
  - codex
  - instructions
  - resume
---

# Codex Instruction Index

## Intent

Provide one entrypoint for Codex to discover repository-specific instructions.

## Precedence

1. `AGENTS.md` (repo-wide behavior and contribution rules)
2. `.codex/instructions/repo-guidelines.md`
3. `.codex/instructions/resume-tailoring.md`
4. `.codex/instructions/content-policy.md`

## Inputs

- User request
- Resume/job-tailoring context from `context/` and `resume/`

## Outputs

- Updated profile, context docs, and role-specific resume drafts

## Constraints

- Keep public-safe content only.
- Preserve timeline consistency across docs.
- Avoid inventing claims or metrics.
