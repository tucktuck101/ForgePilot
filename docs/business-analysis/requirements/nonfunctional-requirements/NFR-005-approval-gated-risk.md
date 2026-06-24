# NFR-005: Approval-Gated Risk

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-005 |
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

Risky decisions must be approved.

## Details

ForgePilot should enforce approval gates for decisions that materially affect product direction, prototype scope, user experience, architecture, external services, credential use, destructive actions, deployment exposures, merges, and final acceptance. Routine implementation details should proceed autonomously, but any action that could cause irreversible changes, incur costs, expose data, or require significant rework must be surfaced to the user for explicit approval.

## Notes

This requirement ensures user control over high-impact decisions while enabling autonomous progress for routine tasks.
