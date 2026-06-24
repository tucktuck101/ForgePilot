# OQ-007: How should stage-aware operating guidance be represented?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-007 |
| Document type | Open Question |
| Status | Open |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-007](../evidence/EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [ASM-006](../assumptions/ASM-006-explicit-stage-context-improves-codex-operation.md), [RSK-008](../risks/RSK-008-wrong-stage-codex-behaviour.md), [Workflows](../workflows.md), [Open Questions Index](index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Question

How should ForgePilot represent stage-aware Codex behaviour in a way that is reusable, token-efficient, GitHub-native, resumable, and safe?

## Resolution

- Owner: Product Owner, with later solution-design and technical-review input.
- Required action: Evaluate how the chosen approach communicates the current work type, expected outputs, constraints, review criteria, quality gates, approval gates, and stop conditions.
- Candidate concepts: stage profiles, role lenses, bounded operating loops, reusable `.agents/skills`, GitHub Issue execution metadata, quality gates, approval gates, or an equivalent mechanism.
- Decision boundary: the candidates are evaluation inputs, not approved designs or implementation commitments.
- Timing: resolve during approved solution design before operating guidance is finalised or implementation work is authorised.
