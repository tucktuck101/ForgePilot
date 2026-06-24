# ASM-006: Explicit stage context improves Codex operation

## Document Metadata

| Field | Value |
|---|---|
| Object ID | ASM-006 |
| Document type | Assumption |
| Status | Unvalidated |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-007](../evidence/EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [RSK-008](../risks/RSK-008-wrong-stage-codex-behaviour.md), [OQ-007](../open-questions/OQ-007-stage-aware-guidance-representation.md), [Assumptions Index](index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Assumption

Codex will operate more safely and consistently when task context clearly identifies the current delivery stage or work type, expected outputs, applicable constraints, quality expectations, approval gates, and stop conditions.

## Validation

Test during representative future delivery scenarios spanning discovery through context recovery. Compare whether Codex produces the expected artefacts, observes applicable gates and stop conditions, and avoids actions belonging to a later or different stage. If the assumption is false, revise the operating-model need and affected risks before finalising a solution.
