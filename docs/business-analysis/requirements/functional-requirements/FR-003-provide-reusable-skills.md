# FR-003: Provide reusable skills

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-003 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-003](../../discovery/stakeholder-needs/SN-003-repository-onboarding.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall include reusable Codex skills stored under the `.agents/skills/` directory. Each skill defines a repeatable workflow that Codex can follow when performing specific tasks during the delivery process.

## Details

The system relies on a modular set of skills to avoid repeating long instructions. Each skill:

- Resides under `.agents/skills/` with its own folder and `SKILL.md` file.
- Has a clear trigger or use case (e.g., discovery interview, solution design, sprint execution, verification, deployment preparation).
- Lists step-by-step instructions, expected outputs, stop conditions, and approval gates.
- References relevant documentation in the `docs/` directory rather than duplicating content.

This requirement ensures that common workflows are encapsulated and maintainable, supporting efficient and consistent behavior across projects.

## Acceptance Criteria

- There is a `.agents/skills/` directory in the repository.
- Each reusable workflow has its own folder and `SKILL.md` file within `.agents/skills/`.
- Skills clearly define their purpose, trigger, steps, outputs, and stop conditions.
- Skills reference documentation instead of duplicating it.
- Skills avoid storing project-specific or transient state.

## Notes

This requirement complements FR-002 (`AGENTS.md`) by storing detailed instructions in separate skill files, keeping the main guidance file concise.
