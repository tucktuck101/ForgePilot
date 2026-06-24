# persona-001: Solo Builder / Product Owner

## Document Metadata

| Field | Value |
|---|---|
| Object ID | persona-001 |
| Document type | Persona |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-001](../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [Personas Index](./index.md) |
| Related objects | [Personas Index](./index.md), [SN-001](../discovery/stakeholder-needs/SN-001-rapid-prototype-delivery.md), [TU-001](../discovery/target-users/TU-001-solo-builder-product-owner.md) |
| Update rule | Update when this persona changes materially |

## Profile

The Solo Builder is the primary human user of ForgePilot. They have app or software ideas and want to rapidly turn those ideas into working prototypes without manually managing every step of software delivery. They may have technical knowledge but want Codex to handle discovery, planning, implementation, testing, documentation, and deployment preparation.

## Goals

- Turn vague ideas into working prototypes.
- Use a reusable GitHub template repo for new or existing projects.
- Avoid manually writing setup prompts for every project.
- Minimise micromanagement of routine development work.
- Maintain control over product direction, risk, cost, secrets, deployment, and acceptance.
- Resume work safely across Codex sessions when token limits are hit.
- Use GitHub Issues and pull requests as the structured delivery workflow.

## Pain Points

- Prototype ideas often stall before implementation.
- Manual discovery, ticketing, and planning are time‑consuming.
- AI or Codex sessions can lose context.
- Token limits interrupt long tasks.
- Existing repos may have inconsistent structure or tooling.
- It is hard to know when to intervene versus letting Codex act autonomously.

## Needs

- Chat-driven discovery with one question at a time.
- A structured template with clear docs and examples.
- GitHub Issues as the executable backlog.
- A pull‑request‑per‑sprint workflow.
- Clear approval gates at meaningful decision points.
- Context recovery via project memory and resume briefs.
- A final handoff package with instructions, limitations, and future backlog.

## Notes

This persona represents the typical user who initiates projects and interacts with Codex to deliver prototypes. They often wear multiple hats, including client and maintainer, but their primary focus is on bringing ideas to life efficiently.
