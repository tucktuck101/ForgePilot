# persona-003: Client / Approval Authority

## Document Metadata

| Field | Value |
|---|---|
| Document type | Persona |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Personas Index](./index.md) |
| Update rule | Update when this persona changes materially |

## Profile

The Client or Approval Authority is the decision‑maker who reviews and approves critical aspects of the project. They may be the same person as the Solo Builder, but they adopt a different role when determining product direction, approving scope, choosing architecture, sanctioning external services or credentials, authorising deployment, merging pull requests, and accepting the final prototype.

## Goals

- Approve major product and scope decisions.
- Approve or reject material UX or architecture choices.
- Control cost, complexity, security, and vendor lock‑in.
- Prevent accidental exposure or data loss.
- Decide whether to accept, iterate, harden, deploy, or stop the project.

## Pain Points

- Too many approval prompts reduce autonomy and productivity.
- Too few approval prompts increase risk and unintended consequences.
- Technical trade‑offs can be difficult to evaluate without context.
- Conflict resolution in existing repos may require nuanced judgement.
- Deployment and secrets decisions can have real financial or legal implications.

## Needs

- Clear approval requests with concise summaries, recommendations, alternatives, and risks.
- Links to relevant documents, issues, or ADRs for context.
- The ability to approve, revise, or reject with confidence.
- An acceptance checklist to evaluate the final handoff.
- Confidence that routine work proceeds autonomously and approval is only requested at meaningful gates.

## Notes

This persona ensures that user oversight is preserved in critical moments. Structuring approval requests well helps maintain trust and efficiency in the delivery process.
