---
id: content-policy-mirror
title: Public Content Policy (Codex Mirror)
source_files:
  - context/README.md
  - context/maintenance-guide.md
audience: ai-agent
last_synced: 2026-04-24
sync_mode: manual
tags:
  - privacy
  - policy
  - consistency
---

# Public Content Policy (Codex Mirror)

## Intent

Prevent profile drift, privacy leaks, and unsupported claims.

## Constraints

- Public-safe content only.
- No personal phone numbers or private identifiers.
- No sensitive internal business details.
- Quantified outcomes must be true and shareable.

## Consistency Rules

- Every major resume bullet should map to at least one Evidence ID.
- Dates and titles must match across all files.
- Add new outcomes as new evidence entries instead of rewriting history.

## Drift Controls

- Refresh role playbook opening lines when role focus changes.
- Refresh skill-depth tags when tooling changes.
- Re-run one sample tailoring prompt per role after substantial updates.

