# Maintenance Guide

Use this checklist whenever experience, projects, or goals change.

## Update flow

1. Update `master-profile.md` timeline first.
2. Add or revise evidence blocks with measurable outcomes.
3. Re-map role fit tags in evidence blocks.
4. Update role playbooks only after the master profile is correct.
5. Re-run one sample tailoring prompt per role to validate output quality.

## Quality rules

- Every major resume bullet should map to at least one Evidence ID.
- Keep dates and titles exactly consistent across files.
- Use only public-safe details.
- Do not duplicate weak bullets across all role playbooks.

## Drift checks

- If a new role starts, refresh top 3 positioning lines for every playbook.
- If tooling stack changes, refresh skill-depth tags in master profile.
- If new outcomes appear, add them as new Evidence IDs instead of editing old history.

## Versioning note

When making substantial updates, commit with messages like:

- `Update master profile for <new role/timeline>`
- `Refresh AI and DevOps playbooks with new evidence`
- `Revise tailoring prompts for ATS constraints`
