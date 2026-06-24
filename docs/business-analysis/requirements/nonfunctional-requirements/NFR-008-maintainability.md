# NFR-008: Maintainability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-008 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must be maintainable.

## Details

The system must be designed with clear separation of concerns: agent operating instructions belong in `AGENTS.md`, reusable workflows reside in `.agents/skills/`, project artefacts live under `docs/`, and scripts and CI configuration are in dedicated locations. Docs should follow a consistent doc‑object style. Skills should be small and reusable. Versions and changelogs must track template evolution. This structure ensures that the template is easy to evolve and maintain over time.

## Notes

A maintainable template reduces complexity for future updates and makes it easier for both humans and Codex to understand the project's organisation.
