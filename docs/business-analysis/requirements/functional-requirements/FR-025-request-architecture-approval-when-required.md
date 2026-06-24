# FR-025: Request architecture approval when required

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-025 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

When the solution design involves meaningful trade-offs or high-impact choices, ForgePilot shall request human approval before finalising the architecture or tech-stack decision.

## Details

Examples of decisions that warrant approval include:

- Choosing between managed versus self-hosted databases or services.
- Selecting a cloud platform that incurs costs or long-term commitments.
- Adopting frameworks with security or vendor lock-in implications.
- Deciding on significant schema or data model structures.

For each such decision, Codex should summarise the rationale, alternatives, pros and cons, and request the user’s approval before proceeding.

## Acceptance Criteria

- Codex identifies decisions that require approval based on cost, security, complexity, or reversibility.
- A clear approval request is made to the user with relevant information.
- The user’s decision is recorded before implementation continues.

## Notes

This requirement aligns with the overall approval gate policy and ensures user control over decisions that could materially affect the project.
