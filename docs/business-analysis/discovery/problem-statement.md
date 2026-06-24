# DISC-002: Problem Statement

## Document Metadata

| Field | Value |
|---|---|
| Object ID | DISC-002 |
| Document type | Problem Statement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation and linked evidence |
| Source need(s) | [SN-001](stakeholder-needs/SN-001-rapid-prototype-delivery.md), [SN-002](stakeholder-needs/SN-002-safe-autonomous-operation.md), [SN-005](stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](evidence/EVD-002-existing-business-analysis-corpus.md), [EVD-003](evidence/EVD-003-repository-gap-observation.md) |
| Related objects | [Current State](current-state.md), [Target Users](target-users/index.md), [Success Criteria](success-criteria/index.md) |
| Update rule | Update when this object or its supporting evidence changes materially |

## Problem

Solo builders and small product owners lack a reusable, repository-native operating model that lets Codex perform the heavy work of software discovery and prototype delivery without either requiring continuous micromanagement or taking material decisions without human control.

## Symptoms

- Discovery, planning, ticketing, testing, documentation, and handoff require repeated manual coordination.
- Repository guidance and delivery state are often fragmented or conversation-bound.
- Users must choose between supervising routine work and accepting unsafe autonomy.
- Context limits make long-running work expensive to reconstruct.

## Root Causes

- No standard adaptive process joins discovery, approval, design, delivery, validation, and handoff.
- Product needs, evidence, requirements, decisions, and work are not consistently linked.
- Approval boundaries are commonly implicit rather than machine-readable.
- Large monolithic artefacts increase retrieval cost for agents.

## Impact

- Slower movement from idea to validated prototype.
- Rework when product direction or scope is misunderstood.
- Risk of destructive changes, credential exposure, unintended cost, or premature deployment.
- Poor continuity and maintainability across sessions and reviewers.

## Desired Outcome

A user can delegate routine prototype delivery to Codex while retaining explicit control over material choices, with compact and traceable repository artefacts that support safe continuation and handoff.

## Evidence Limits

The problem is supported by stakeholder intent and repository analysis. External user research and quantitative baselines are not yet available and must not be inferred.
