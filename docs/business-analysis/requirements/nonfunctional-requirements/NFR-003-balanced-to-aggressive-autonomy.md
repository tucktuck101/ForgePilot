# NFR-003: Balanced-to-Aggressive Autonomy

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

ForgePilot shall default to balanced-to-aggressive autonomy.

## Details

The system should autonomously plan, implement, test, document, and manage GitHub workflows for routine tasks without requiring frequent human intervention. It should only pause and request approval when reaching defined approval gates, encountering high-risk or destructive operations, or requiring human decisions about product direction, cost, or credential usage. The default mode should be more autonomous than conservative, but not so aggressive that it performs risky or irreversible actions without permission.

## Notes

This requirement sets the overall autonomy level for Codex as a delivery agent, balancing productivity with safety and user control.
