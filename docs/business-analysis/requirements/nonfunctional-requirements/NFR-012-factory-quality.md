# NFR-012: Factory Quality

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

The ForgePilot template itself must be validated regularly.

## Details

ForgePilot should include scripts and continuous integration workflows that validate the integrity of the template. Validation should check that required files and folders exist, that skills and templates are present and structurally valid, that documentation uses the correct metadata format, and that no secrets or placeholder content are accidentally committed. Factory validation helps ensure that future updates do not introduce regressions or break the template’s assumptions.

## Notes

Maintaining high factory quality reduces the risk of errors when applying the template to new or existing projects.
