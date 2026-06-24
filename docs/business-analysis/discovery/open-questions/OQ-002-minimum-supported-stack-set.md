# OQ-002: What is the minimum validated stack set?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-002 |
| Document type | Open Question |
| Status | Answered; pending GATE-003 |
| Priority | Should |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation, Product Owner answer dated 2026-06-25, and linked evidence |
| Source need(s) | [SN-004](../stakeholder-needs/SN-004-adaptive-environments-and-stacks.md) |
| Evidence | [EVD-004](../evidence/EVD-004-user-research-gap.md) |
| Related objects | [Open Questions Index](index.md), [Prototype Scope](../scope.md), [GATE-003](../approval-gates/GATE-003-prototype-scope-approval.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Question

What is the minimum validated stack set?

## Resolution

- Answer: The minimum proposed validation set is Node/TypeScript, Python, Go, static sites, Docker-based projects, and an unknown-stack fallback.
- Decision: Use the expanded representative set rather than limiting the first validation set to Node/TypeScript, Python, and unknown-stack handling.
- Decision date: 2026-06-25.
- Decision reference: Product Owner selected option B in the Codex open-question working session dated 2026-06-25.

## Consequences and Approval Boundary

- The expanded set increases fixture, validation, and maintenance effort.
- Docker validation covers container-aware operation and may overlap with a language or static-site fixture; it does not create a claim of compatibility with every containerised stack.
- The unknown-stack fixture must demonstrate conservative detection, documented assumptions, and safe escalation rather than successful stack-specific automation.
- This answer is a proposed prototype-scope input. GATE-003 must approve, revise, or reject its inclusion before implementation planning or prototype construction.
- No broad compatibility claim is permitted from this bounded validation set.
