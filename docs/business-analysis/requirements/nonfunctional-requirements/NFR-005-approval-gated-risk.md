# NFR-005: Approval-Gated Risk

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

Risky decisions must be approved.

## Details

ForgePilot should enforce approval gates for decisions that materially affect product direction, prototype scope, user experience, architecture, external services, credential use, destructive actions, deployment exposures, merges, and final acceptance. Routine implementation details should proceed autonomously, but any action that could cause irreversible changes, incur costs, expose data, or require significant rework must be surfaced to the user for explicit approval.

## Notes

This requirement ensures user control over high-impact decisions while enabling autonomous progress for routine tasks.
