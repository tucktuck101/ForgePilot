# NFR-003: Balanced-to-Aggressive Autonomy

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-003 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-002](../../discovery/stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

ForgePilot shall default to balanced-to-aggressive autonomy.

## Details

The system should autonomously plan, implement, test, document, and manage GitHub workflows for routine tasks without requiring frequent human intervention. It should only pause and request approval when reaching defined approval gates, encountering high-risk or destructive operations, or requiring human decisions about product direction, cost, or credential usage. The default mode should be more autonomous than conservative, but not so aggressive that it performs risky or irreversible actions without permission.

## Notes

This requirement sets the overall autonomy level for Codex as a delivery agent, balancing productivity with safety and user control.
