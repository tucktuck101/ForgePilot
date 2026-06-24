# NFR-006: Token Efficiency

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-006 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot shall minimise token usage.

## Details

The system must optimise for minimal context consumption. Codex should read only the necessary files, link to detailed artefacts instead of duplicating content, maintain a compact project memory, and update memory by overwriting stale facts rather than appending logs. The system should summarise decisions and avoid copying large content into notes. When token pressure is detected, it must pause gracefully and create a resume brief rather than failing abruptly.

## Notes

Reducing token usage improves reliability and efficiency, especially for long-running tasks that span multiple Codex sessions.
