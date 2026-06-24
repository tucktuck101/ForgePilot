# SC-010: Token-efficient documentation retrieval

## Document Metadata

| Field | Value |
|---|---|
| Object ID | SC-010 |
| Document type | Success Criterion |
| Status | Unvalidated |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-008](../stakeholder-needs/SN-008-continuity-across-context-limits.md), [SN-011](../stakeholder-needs/SN-011-human-consumable-documentation.md) |
| Evidence | [EVD-006](../evidence/EVD-006-dual-purpose-documentation-intent.md) |
| Related objects | [SC-006](SC-006-context-efficient-navigation.md), [FR-070](../../requirements/functional-requirements/FR-070-link-to-detailed-artefacts.md), [NFR-006](../../requirements/nonfunctional-requirements/NFR-006-token-efficiency.md) |
| Update rule | Update when the selective-retrieval target or measurement method changes materially |

## Criterion

Codex can complete a bounded documentation task by starting from an issue, compact index, or summary and loading only directly relevant linked artefacts.

## Measurement

Run a representative documentation task in a fresh session. Target: successful completion without ingesting the complete documentation corpus and without missing required authoritative context.
