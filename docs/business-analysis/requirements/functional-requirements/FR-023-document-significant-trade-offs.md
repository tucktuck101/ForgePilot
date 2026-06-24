# FR-023: Document significant trade-offs

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
| Update rule | Update when this functional requirement changes materially |

## Summary

For decisions that involve significant trade-offs, such as selecting a database, external service, or architectural pattern, Codex must document the rationale, alternatives, and consequences.

## Details

When Codex recommends a choice that affects cost, security, maintenance, or vendor lock-in, it should:

- Summarise the chosen option and why it is recommended.
- List at least one alternative and reasons it was not chosen.
- Describe the implications of the decision (positive and negative consequences).

This information should be recorded either in design documents or as part of an Architecture Decision Record (ADR).

## Acceptance Criteria

- Significant technical decisions include rationale, alternatives, and consequences.
- Documentation is placed in the appropriate design document or ADR.
- Stakeholders can understand why a choice was made and what trade-offs were considered.

## Notes

This requirement improves transparency and helps future maintainers understand past decisions. It aligns with FR-024 (create ADRs).
