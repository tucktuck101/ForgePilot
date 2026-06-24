# NFR-002: Chat-Driven Operation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | NFR-002 |
| Document type | Nonfunctional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Nonfunctional Requirements Index](index.md) |
| Related objects | [Nonfunctional Requirements Index](index.md), [SN-001](../../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Update rule | Update when this nonfunctional requirement changes materially |

## Summary

The system must operate through chat.

## Details

All interactions with ForgePilot should be conducted via chat, either through the Codex CLI chat interface or the Codex chat window. No separate graphical user interface or web application is required for version 1. Commands, prompts, approvals, and outputs should be delivered in conversational form. Future versions may integrate additional interfaces, but chat must remain the primary interaction mode.

## Notes

This requirement ensures that the user can drive the system entirely through text-based interactions without needing to context-switch into another UI.
