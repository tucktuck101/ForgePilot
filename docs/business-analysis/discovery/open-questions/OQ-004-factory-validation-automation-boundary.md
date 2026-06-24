# OQ-004: Which factory checks must be automated?

## Document Metadata

| Field | Value |
|---|---|
| Object ID | OQ-004 |
| Document type | Open Question |
| Status | Answered; pending GATE-003 |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation, Product Owner answer dated 2026-06-25, and linked evidence |
| Source need(s) | [SN-006](../stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-004](../evidence/EVD-004-user-research-gap.md) |
| Related objects | [Open Questions Index](index.md), [Prototype Scope](../scope.md), [GATE-003](../approval-gates/GATE-003-prototype-scope-approval.md), [FR-047](../../requirements/functional-requirements/FR-047-include-factory-validation.md), [FR-050](../../requirements/functional-requirements/FR-050-validate-doc-object-metadata.md), [FR-051](../../requirements/functional-requirements/FR-051-validate-no-secrets-are-committed.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Question

Which factory checks must be automated?

## Resolution

- Answer: Automate checks for required structure, object metadata and IDs, index consistency, relative links, template/example separation, and secret safety.
- Decision: Keep semantic quality, evidence sufficiency, and approval-boundary judgments as explicit human review responsibilities.
- Decision date: 2026-06-25.
- Decision reference: Product Owner selected option A in the Codex open-question working session dated 2026-06-25.

## Automation Boundary

- Required structure includes mandatory files and directories plus the expected presence and structural shape of skills and templates.
- Metadata checks include required fields, unique IDs, valid priorities and statuses where constrained, and resolvable traceability links.
- Index checks must detect missing, duplicate, stale, or incorrectly linked live objects.
- Template/example checks must keep authoring aids and examples separate from live project truth.
- Secret checks must detect prohibited secret-bearing files and likely credential values while using placeholders safely.
- Automation may report semantic-review prompts, but it must not infer evidence quality, approve a gate, or replace human judgment about material scope or design decisions.
- GATE-003 must approve, revise, or reject this implementation boundary before planning or prototype construction.
