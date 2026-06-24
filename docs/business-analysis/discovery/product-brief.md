# DISC-001: ForgePilot Product Brief

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-001 |
| Document type | Product Brief |
| Status | Pending approval |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-003](stakeholder-needs/SN-003-repository-onboarding.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](evidence/EVD-002-existing-business-analysis-corpus.md) |
| Related objects | [GATE-002](approval-gates/GATE-002-product-brief-approval.md), [Scope](scope-items/index.md), [Options](options/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Summary

ForgePilot is a reusable GitHub repository template intended to help Codex move a software idea from discovery to a tested prototype and final handoff with minimal routine user coordination and explicit human control at material decisions.

## Product Goal

Enable a user to move from a vague idea to an approved, working prototype through a repository-native, chat-driven process that remains safe, traceable, resumable, adaptable, and maintainable.

## Problem and Users

- Problem: [Problem Statement](problem-statement.md).
- Current state: [Current State](current-state.md).
- Target users: [Target Users Index](target-users/index.md).
- Stakeholder authority: [Stakeholder Map](stakeholder-map.md).
- Stakeholder needs: [Stakeholder Needs Index](stakeholder-needs/index.md).

## Proposed Direction

The current recommendation is [OPT-002: Reusable GitHub template](options/OPT-002-reusable-github-template.md). This direction remains provisional until GATE-001 is approved.

## Prototype Intent

The prototype should test whether repository instructions, atomic doc objects, explicit approvals, validation, and GitHub-native delivery conventions are sufficient to support the documented discovery-to-handoff workflow.

## Scope and Outcomes

- Consolidated prototype scope: [Prototype Scope](scope.md).
- Atomic scope items: [Scope Items Index](scope-items/index.md).
- Current and target workflows: [Workflow Analysis](workflows.md).
- Prototype hypotheses: [Prototype Hypotheses Index](prototype-hypotheses/index.md).
- Value hypotheses: [Value Hypotheses Index](value-hypotheses/index.md).
- Value and success model: [Value and Success Definition](value-and-success-criteria.md).
- Atomic success criteria: [Success Criteria Index](success-criteria/index.md).
- Risks, assumptions, and questions: [Risks](risks/index.md), [Assumptions](assumptions/index.md), [Open Questions](open-questions/index.md).

## Operating Principles

- Use compact indexes and atomic related objects.
- Keep durable project knowledge in version-controlled Markdown.
- Use one adaptive process across new and existing repositories.
- Prefer free, open-source, local, and GitHub-native tools.
- Act autonomously within explicit approval and safety boundaries.
- Preserve state for safe continuation across context limits.

## Approval State

- Options and direction: Pending GATE-001.
- Product brief: Pending GATE-002.
- Prototype scope: Pending GATE-003.
- Solution design is blocked while GATE-002 is pending.
- Implementation is blocked while GATE-002 or GATE-003 is pending.
- Later material decisions remain governed by the [approval operating policy](approval-gates/operating-policy.md).
