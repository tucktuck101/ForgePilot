# NFR-009: Portability

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

The system must be portable across different repositories.

## Details

ForgePilot should work with new empty repositories, newly created repositories, existing partially built repositories, and mature repositories. It should detect existing structure, tooling, scripts, tests, and documentation and adapt its behaviour accordingly. When installing the template into an existing repo, it must handle conflicts carefully and avoid overwriting valuable files without approval. Portability also means that the template should not rely on platform-specific features unless clearly documented and approved.

## Notes

Portability ensures that the system can be reused across a variety of projects without manual reconfiguration.
