# persona-006: ForgePilot Maintainer

## Document Metadata

| Field | Value |
|---|---|
| Object ID | persona-006 |
| Document type | Persona |
| Status | Draft |
| Priority | Could |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Personas Index](./index.md) |
| Related objects | [Personas Index](./index.md), [SN-010](../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md), [TU-006](../discovery/target-users/TU-006-forgepilot-maintainer.md) |
| Update rule | Update when this persona changes materially |

## Profile

The ForgePilot Maintainer is responsible for updating and improving the ForgePilot template itself. They care about template quality, versioning, examples, skills, scripts, validation, and documentation. This may be the user, Codex, or both.

## Goals

- Keep the template reliable and up to date.
- Maintain a version file and changelog.
- Validate skills, templates, scripts, docs, and CI workflows.
- Improve support for additional stacks and environments.
- Prevent template regressions and ensure examples are separate from project truth.

## Pain Points

- The template can drift or degrade over time without maintenance.
- Example artefacts may be mistaken for live project artefacts if not clearly marked.
- Scripts and validation may become stale as new stacks are added.
- Skills may duplicate guidance unnecessarily.
- Changes may inadvertently break bootstrap behaviour or conventions.

## Needs

- A clear versioning scheme recorded in `VERSION`.
- A comprehensive `CHANGELOG.md` documenting template changes.
- Factory validation scripts and CI workflows.
- Well‑separated examples with clear markings.
- Template tests that ensure required files and structure.
- A maintenance backlog for improvements and new stack support.

## Notes

By maintaining the template as a product, this persona ensures ForgePilot remains reliable and useful as technology and user needs evolve.
