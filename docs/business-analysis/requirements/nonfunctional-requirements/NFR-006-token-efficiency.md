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
| Source need(s) | [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-011](../../discovery/stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-006](../../discovery/evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-008](../../discovery/stakeholder-needs/SN-008-continuity-across-context-limits.md), [SC-010](../../discovery/success-criteria/SC-010-token-efficient-documentation-retrieval.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot shall minimise token usage.

## Details

The system must optimise for minimal context consumption. The documentation corpus should operate as an indexed, linked knowledge graph: Codex starts from issues, compact indexes, summaries, or current-state records and loads only directly relevant objects. Detailed artefacts should be linked instead of duplicated, project memory should remain compact, and stale facts should be replaced rather than accumulated as logs. When token pressure is detected, Codex must pause gracefully and create a resume brief rather than failing abruptly.

## Acceptance Criteria

- A fresh-session documentation task completes from an issue, index, or summary plus directly linked objects.
- The task does not require loading the complete documentation corpus.
- Detailed content is stored once and referenced by relative link from summaries and work records.
- Required context is not omitted as a consequence of minimising token use.

## Notes

Reducing token usage improves reliability and efficiency, especially for long-running tasks that span multiple Codex sessions.
