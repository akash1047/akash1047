# Tailoring Prompts

These prompts turn the context library into role-specific resume drafts.

## General constraints for all prompts

- Use facts only from this repository context.
- Preserve timeline accuracy and company/role titles exactly.
- Prefer quantified outcomes when available.
- Keep output ATS-friendly: clean sections, no tables, no icons.
- Do not include phone number or sensitive internal details.

## Prompt 1: Role-targeted resume draft

```text
You are writing a one-page ATS-friendly resume.

Inputs:
- Role target: <Frontend|Backend|DevOps|AI|Full Stack>
- Job description: <paste JD>
- Context files:
  - context/master-profile.md
  - context/role-playbooks/<role>.md

Instructions:
1) Build a tailored headline and 3-line summary aligned to the target role.
2) Select 4-6 highest-relevance Evidence IDs from master profile.
3) Write experience bullets prioritizing measurable outcomes.
4) Keep only skills relevant to the JD and role playbook priorities.
5) Return: Headline, Summary, Experience, Projects, Skills.
6) Keep it truthful; do not invent tools, metrics, or responsibilities.
```

## Prompt 2: Gap analysis before writing

```text
Given:
- Target role and JD
- context/master-profile.md
- one role playbook

Produce:
1) Matching strengths (ranked)
2) Missing signals (skills/evidence gaps)
3) Suggested bullet emphasis changes
4) Skills to de-prioritize for this JD
5) Final recommendation: fit level (high/medium/low)
```

## Prompt 3: Bullet rewrite optimizer

```text
Rewrite these resume bullets for <target role> using only repository context.
Rules:
- Start each bullet with a strong action verb.
- Include stack only when it adds relevance.
- Prefer outcome phrasing (impact, speed, reliability, scale).
- Keep each bullet under 24 words.
Return 2 variants per bullet: ATS-safe and recruiter-friendly.
```

## Prompt 4: Final consistency audit

```text
Audit the tailored resume against context/master-profile.md.
Check:
- timeline consistency
- title/company consistency
- claim validity
- role relevance
- ATS readability

Return:
- pass/fail
- exact lines needing correction
- corrected replacement lines
```
