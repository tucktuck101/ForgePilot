# OQ-007: How should stage-aware operating guidance be represented?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-007 |
| Document type | Open Question |
| Status | Preferred proposal recorded; design approval pending |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation, Product Owner answer dated 2026-06-25, and linked evidence |
| Source need(s) | [SN-002](../stakeholder-needs/SN-002-safe-autonomous-operation.md) |
| Evidence | [EVD-007](../evidence/EVD-007-stage-aware-operating-guidance-need.md) |
| Related objects | [ASM-006](../assumptions/ASM-006-explicit-stage-context-improves-codex-operation.md), [RSK-008](../risks/RSK-008-wrong-stage-codex-behaviour.md), [Workflows](../workflows.md), [Open Questions Index](index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Question

How should ForgePilot represent stage-aware Codex behaviour in a way that is reusable, token-efficient, GitHub-native, resumable, and safe?

## Resolution

- Preferred proposal: Use a layered representation consisting of concise adaptive workflow chunks in `AGENTS.md`, detailed reusable skills for repeatable work types, and GitHub Issue metadata identifying the current chunk, required outputs, checks, approval gates, and stop conditions.
- Alternative considered: Standalone stage-profile documents containing the complete guidance, with issues linking to the active profile; not preferred because it concentrates guidance into larger profiles and increases duplication and context-loading risk.
- Decision date: 2026-06-25.
- Decision reference: Product Owner selected option A in the Codex open-question working session dated 2026-06-25.

## Consequences and Approval Boundary

- `AGENTS.md` provides the durable repository-level routing model and must remain concise.
- Reusable `.agents/skills/` hold detailed workflows with clear triggers, outputs, quality checks, approval gates, and stop conditions.
- GitHub Issues carry execution-specific state and links without duplicating the authoritative workflow instructions.
- Project facts and transient delivery state remain under `docs/` or the linked issue rather than being embedded in reusable skills.
- Approved solution design must define the metadata schema, routing rules, precedence, fallback behaviour, stale-state detection, and scenario-based validation against SC-013.
- This preferred proposal does not authorise creation of the skills, issue schema, automation, or other implementation while GATE-002 and applicable scope or design approvals remain pending.
