# FR-029: Define GitHub issue structure

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-029 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

Each delivery issue should follow a consistent structure to communicate the goal, context, and criteria for completion. This makes tasks clear and ensures proper tracking.

## Details

An issue should include the following fields:

- **Title**: A concise description of the task or feature.
- **Goal**: The purpose or desired outcome.
- **Context**: Links to relevant requirements, user stories, design documents, and any background information.
- **Acceptance Criteria**: Specific conditions that must be met for the work to be considered done.
- **Dependencies**: Other issues or tasks that must be completed first.
- **Risk Level**: A brief assessment of the complexity or risk associated with the task.
- **Approval Gates**: Any required approvals before work can proceed.
- **Test Expectations**: The tests that should be added or updated.
- **Definition of Done**: A brief recap of the general DoD criteria (e.g., tests pass, docs updated).

This structure may be represented as a template that Codex fills out when generating issues.

## Acceptance Criteria

- Issues created by Codex include all of the above fields.
- Fields are clearly labelled and populated with appropriate content.
- Issue templates or comments guide the user on what each field means.

## Notes

A consistent issue structure aids in planning, review, and automated tracking of work. It also facilitates token-efficient processing by Codex when reading and updating issues.
