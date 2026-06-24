# FR-032: Select sprint scope adaptively

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-032 |
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

ForgePilot shall allow Codex to choose sprint size based on the nature of the work, adjusting between small and large scopes to balance quality, risk, and token efficiency.

## Details

- Small sprints are recommended when requirements are unclear, risk is high, files are unfamiliar, tests are failing, or security/data/auth/deployment is involved.
- Larger sprints may be used when tasks are clear, repetitive, low-risk, documentation or configuration-heavy, or when conventions are strong.
- Codex should explain the rationale for choosing the sprint size and how it aligns with project goals and token limitations.

## Acceptance Criteria

- Sprint size varies based on defined criteria.
- Rationale for sprint size is documented in `docs/business-analysis/delivery/current-sprint.md` or issue comments.
- Sprint planning decisions are transparent and justifiable.

## Notes

Adapting sprint scope helps manage complexity and ensures that tasks are completed efficiently without sacrificing quality.
