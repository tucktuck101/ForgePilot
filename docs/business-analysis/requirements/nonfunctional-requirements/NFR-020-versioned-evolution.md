# NFR-020: Versioned Evolution

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-020 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Could |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-010](../../discovery/stakeholder-needs/SN-010-maintainable-versioned-template.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot must manage its own evolution through versioning.

## Details

The template should include a `VERSION` file and a `CHANGELOG.md` documenting changes to its structure, skills, scripts, documentation, examples, and policies. Every significant update to the template should increment the version number and add an entry to the changelog explaining what changed and why. This version discipline helps users and Codex understand which template version they are using and what differences exist between versions.

## Notes

Versioned evolution provides transparency and allows users to upgrade intentionally rather than unexpectedly inheriting changes.
