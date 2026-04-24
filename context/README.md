# Career Context System

This directory is a public-safe knowledge base for generating role-specific resumes from one source of truth.

## What this is for

- Maintain one canonical profile of your background.
- Tailor resumes quickly for different roles without rewriting from scratch.
- Keep claims evidence-backed and timeline-consistent.

## Files

- `master-profile.md`: Canonical career facts, timeline, strengths, and evidence blocks.
- `role-playbooks/*.md`: Positioning strategy and bullet priorities per role.
- `tailoring-prompts.md`: Prompt-ready workflows to generate targeted drafts.
- `maintenance-guide.md`: How to update safely without profile drift.
- AI mirror: `.codex/instructions/resume-tailoring.md` for machine-first parsing.

## Evidence block schema

Use this schema across files to keep content reusable and verifiable.

```text
Evidence ID: E-XXX
Role Fit: Primary=[...], Secondary=[...]
Skill Depth: <working|strong|advanced>
Problem:
Action:
Stack:
Outcome:
Confidence: <high|medium>
Notes:
```

## Privacy rules

- Public-safe content only.
- No personal phone number, private identifiers, or sensitive internal data.
- Quantified outcomes should be true and externally safe to share.
