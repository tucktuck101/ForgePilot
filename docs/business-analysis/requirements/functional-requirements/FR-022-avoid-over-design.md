# FR-022: Avoid over-design

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-022 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

Solution design documents should be lean and focused, providing only the necessary detail to build and test the prototype effectively. ForgePilot should avoid over-engineering or excessive documentation.

## Details

- Design artefacts should prioritise clarity and actionable guidance.
- Documents should avoid duplicating implementation details that will be discovered during sprints.
- The level of detail should match the complexity of the project; straightforward prototypes require less detailed architecture diagrams and design sections.
- When in doubt, err on the side of simplicity and supplement with ADRs for significant trade-offs.

## Acceptance Criteria

- Design documents are concise and do not include unnecessary detail.
- The developer can implement the prototype based on the design without guesswork or extraneous information.
- Stakeholders find the design easy to understand and maintain.

## Notes

This requirement helps manage token usage and ensures that documentation adds value without becoming an overhead.
