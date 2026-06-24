# NFR-008: Maintainability

## Document Metadata

| Field | Value |
|---|---|
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Nonfunctional Requirements Index](../index.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must be maintainable.

## Details

The system must be designed with clear separation of concerns: agent operating instructions belong in `AGENTS.md`, reusable workflows reside in `.agents/skills/`, project artefacts live under `docs/`, and scripts and CI configuration are in dedicated locations. Docs should follow a consistent doc‑object style. Skills should be small and reusable. Versions and changelogs must track template evolution. This structure ensures that the template is easy to evolve and maintain over time.

## Notes

A maintainable template reduces complexity for future updates and makes it easier for both humans and Codex to understand the project's organisation.
