---
id: resume-tailoring-mirror
title: Resume Tailoring Workflow (Codex Mirror)
source_files:
  - context/tailoring-prompts.md
  - context/maintenance-guide.md
audience: ai-agent
last_synced: 2026-04-24
sync_mode: manual
tags:
  - resume
  - tailoring
  - ats
---

# Resume Tailoring Workflow (Codex Mirror)

## Intent

Generate role-targeted resumes using repository facts only.

## Inputs

- Target role (`frontend`, `backend`, `fullstack`, `devops`, `ai`)
- Job description text
- Context files:
  - `context/master-profile.md`
  - `context/role-playbooks/<role>.md`

## Rules

- Use only facts present in this repository.
- Keep timeline, company, and title strings exact.
- Prefer quantified outcomes where available.
- Keep ATS-friendly formatting (plain sections, no tables/icons).
- Exclude phone numbers, private identifiers, and sensitive internal data.

## Process

1. Run quick gap analysis against JD.
2. Select highest relevance Evidence IDs.
3. Draft role-specific summary and bullets.
4. Optimize bullet wording for impact and brevity.
5. Run final consistency audit against master profile.

## Outputs

- Tailored resume section set: headline, summary, experience, projects, skills.
- Explicit fit statement (`high`/`medium`/`low`) when requested.

