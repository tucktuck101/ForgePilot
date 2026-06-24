# FR-077: Produce Final Handoff

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-077 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-009](../../discovery/stakeholder-needs/SN-009-complete-prototype-handoff.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Related objects | [Functional Requirements Index](index.md), [SN-009](../../discovery/stakeholder-needs/SN-009-complete-prototype-handoff.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system must generate a final handoff document when a prototype is completed.

## Details

Upon completing the prototype, Codex should produce a final handoff artefact at `docs/delivery/final-handoff.md`. This file serves as the definitive record of what was delivered and provides all information required for review, testing, deployment, or continued development. The handoff should be produced only after the post-build acceptance gate has been reached and approved.

## Acceptance Criteria

- A `final-handoff.md` file is created under `docs/delivery/` when the prototype is complete.
- The final handoff document includes all required sections as specified in FR-078, FR-079, and FR-080.
- The handoff is clearly timestamped and linked to the approved scope and acceptance decision.

## Notes

This requirement ensures that the end of a delivery cycle results in a clear, comprehensive package for acceptance and future work.
