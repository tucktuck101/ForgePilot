# NFR-009: Portability

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-009 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-004](../../discovery/stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

The system must be portable across different repositories.

## Details

ForgePilot should work with new empty repositories, newly created repositories, existing partially built repositories, and mature repositories. It should detect existing structure, tooling, scripts, tests, and documentation and adapt its behaviour accordingly. When installing the template into an existing repo, it must handle conflicts carefully and avoid overwriting valuable files without approval. Portability also means that the template should not rely on platform-specific features unless clearly documented and approved.

## Notes

Portability ensures that the system can be reused across a variety of projects without manual reconfiguration.
