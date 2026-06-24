# NFR-019: Repeatable Validation

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

Validation must be repeatable.

## Details

ForgePilot should provide scripts and GitHub Actions workflows that can be run repeatedly to validate both the template and generated projects. Validation should include checking required files and structures, verifying skills and templates, enforcing documentation metadata, scanning for secrets, and running relevant tests, linting, formatting, and builds. The output of validation should be deterministic, and failures should include clear messages to help diagnose issues.

## Notes

Repeatable validation supports consistent quality and helps detect regressions early during template updates or project delivery.
