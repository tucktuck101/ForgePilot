# RSK-008: Wrong-stage Codex behaviour

## Document Metadata

| Field | Value |
|---|---|
| Object ID | RSK-008 |
| Document type | Risk |
| Status | Open |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-007](../evidence/EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [ASM-006](../assumptions/ASM-006-explicit-stage-context-improves-codex-operation.md), [OQ-007](../open-questions/OQ-007-stage-aware-guidance-representation.md), [Risks Index](index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Assessment

- Likelihood/impact: High.
- Owner: Product Owner and ForgePilot Maintainer.
- Failure modes: Codex may implement during analysis, make design decisions before approval, miss quality or approval gates, produce inconsistent artefacts, continue past a required stop condition, or apply unsafe autonomy.
- Mitigation: Record the stage-aware operating need during business analysis, require current work to remain within documented gate boundaries, and evaluate representation options later during approved solution design.
- Design boundary: No candidate mechanism is approved by this mitigation.

## Closure Condition

Close only after an approved solution has been tested across representative stages and evidence shows that expected outputs, quality gates, approval gates, and stop conditions are applied consistently.
