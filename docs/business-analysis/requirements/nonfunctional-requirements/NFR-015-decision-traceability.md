# NFR-015: Decision Traceability

## Document Metadata

| Field | Value |
|---|---|
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

Significant decisions must be traceable.

## Details

When ForgePilot makes or recommends a decision that has long‑term impact—such as architecture, data model, deployment, security, privacy, cost, vendor lock‑in, licensing, major dependencies, or maintainability—it must create an Architecture Decision Record (ADR) or document the decision in sprint notes. ADRs should include context, the decision made, consequences, alternatives considered, and links to related artefacts. Routine decisions should still be documented in sprint notes but do not require formal ADRs.

## Notes

Decision traceability helps future maintainers understand why certain choices were made and provides a basis for revisiting them if conditions change.
