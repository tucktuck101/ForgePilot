# NFR-020: Versioned Evolution

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

ForgePilot must manage its own evolution through versioning.

## Details

The template should include a `VERSION` file and a `CHANGELOG.md` documenting changes to its structure, skills, scripts, documentation, examples, and policies. Every significant update to the template should increment the version number and add an entry to the changelog explaining what changed and why. This version discipline helps users and Codex understand which template version they are using and what differences exist between versions.

## Notes

Versioned evolution provides transparency and allows users to upgrade intentionally rather than unexpectedly inheriting changes.
