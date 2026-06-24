# EVD-007: Stage-aware operating guidance need

## Document Metadata

| Field | Value |
|---|---|
| Object ID | EVD-007 |
| Document type | Evidence |
| Status | Recorded |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | Direct Product Owner instruction dated 2026-06-24 and analysis of the documented delivery workflow |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-007](EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [Current State](../current-state.md), [Workflows](../workflows.md) |
| Update rule | Update when this finding or its supporting evidence changes materially |

## Summary

The Product Owner identified a business/process need for Codex behaviour to vary with the current delivery stage, task type, expected outputs, quality gates, approval gates, and stop conditions. A single generic operating instruction set may not provide enough context to keep discovery, analysis, shaping, design preparation, implementation, validation, pull-request readiness, and context recovery appropriately bounded.

## Reliability and Limitations

- Provenance: direct stakeholder instruction received on 24 June 2026 and consistent with the stage and gate distinctions already documented in ForgePilot.
- Confidence: high that the need should be evaluated; unvalidated that any particular representation will produce the intended outcomes.
- Boundary: stage profiles, role lenses, bounded operating loops, reusable skills, issue metadata, quality gates, and approval gates are candidate concepts only. This evidence does not approve a solution design, implementation mechanism, or prototype-scope change.
