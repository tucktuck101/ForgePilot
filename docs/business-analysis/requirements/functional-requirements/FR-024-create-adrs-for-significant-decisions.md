# FR-024: Create ADRs for significant decisions

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-024 |
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

When a decision affects the architecture, data model, deployment, security, privacy, cost, vendor lock-in, licensing, major dependencies, or long-term maintainability, ForgePilot shall capture it in an Architecture Decision Record (ADR).

## Details

- ADRs should be stored under `docs/business-analysis/decisions/` with a filename pattern like `ADR-####-short-title.md`.
- Each ADR follows a standard structure with sections for Status, Context, Decision, Consequences, Alternatives Considered, and Links.
- ADRs are only created for decisions that are hard to reverse or have long-term impact.
- Routine implementation choices and design variations should be recorded in sprint notes rather than ADRs.

## Acceptance Criteria

- Significant decisions are documented in ADRs.
- ADRs follow the defined structure and naming convention.
- ADRs are linked from the relevant design document or sprint note.

## Notes

This requirement ensures important decisions are traceable and maintainable, supporting transparency and reducing the risk of repeating deliberation in the future.
