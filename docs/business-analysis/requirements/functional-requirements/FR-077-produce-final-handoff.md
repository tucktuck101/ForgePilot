# FR-077: Produce Final Handoff

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Functional Requirements Index](../index.md) |
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