# NFR-004: Safe Defaults

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

ForgePilot must use safe defaults for tools and operations.

## Details

By default, the system should select non-destructive, reversible, local, free, and open‑source tools and workflows wherever possible. It must avoid automatically adopting paid services, external dependencies, or irreversible commands without explicit approval. When a project requires a potentially risky or costly option, the system should recommend alternatives and ask for permission before proceeding.

## Notes

This requirement reduces accidental costs, security issues, and data loss by ensuring the default behaviour is conservative when side effects are unclear or potentially harmful.
