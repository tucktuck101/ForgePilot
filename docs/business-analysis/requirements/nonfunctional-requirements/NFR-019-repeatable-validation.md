# NFR-019: Repeatable Validation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-019 |
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

Validation must be repeatable.

## Details

ForgePilot should provide scripts and GitHub Actions workflows that can be run repeatedly to validate both the template and generated projects. Validation should include checking required files and structures, verifying skills and templates, enforcing documentation metadata, scanning for secrets, and running relevant tests, linting, formatting, and builds. The output of validation should be deterministic, and failures should include clear messages to help diagnose issues.

## Notes

Repeatable validation supports consistent quality and helps detect regressions early during template updates or project delivery.
