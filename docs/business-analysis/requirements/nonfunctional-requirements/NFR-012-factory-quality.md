# NFR-012: Factory Quality

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-012 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-006](../../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

The ForgePilot template itself must be validated regularly.

## Details

ForgePilot should include scripts and continuous integration workflows that validate the integrity of the template. Validation should check that required files and folders exist, that skills and templates are present and structurally valid, that documentation uses the correct metadata format, and that no secrets or placeholder content are accidentally committed. Factory validation helps ensure that future updates do not introduce regressions or break the template’s assumptions.

## Notes

Maintaining high factory quality reduces the risk of errors when applying the template to new or existing projects.
