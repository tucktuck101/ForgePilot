# persona-002: Codex Delivery Agent

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

The Codex Delivery Agent is the autonomous system operating inside the repository. It reads `AGENTS.md`, uses reusable skills, inspects the repository, interviews the user, creates artefacts, manages issues and branches, implements scoped sprints, runs tests, opens draft pull requests, prepares deployment, and stops for human approval when required.

## Goals

- Understand the repository structure quickly.
- Follow durable repo instructions from `AGENTS.md`.
- Use reusable skills to avoid repeating long prompts.
- Create and maintain project artefacts in Markdown.
- Use GitHub Issues as the work queue and generate one pull request per sprint.
- Implement tasks autonomously while respecting approval gates.
- Maintain enough context to resume safely across sessions.
- Avoid unsafe or unapproved actions.

## Pain Points

- Missing or scattered context can lead to confusion.
- Unknown stacks require fallback logic.
- Large context windows consume tokens quickly.
- Approval gates may be unclear or missing.
- Validation commands might be absent or stack‑specific.
- Risk of overwriting existing files without approval.
- Example artefacts might be mistaken for project truth.

## Needs

- A concise `AGENTS.md` with clear operating rules.
- Reusable skills stored under `.agents/skills/`.
- Compact project memory and sprint files for state persistence.
- Issue and PR templates to standardise work.
- Conflict detection and resolution guidelines.
- A clear approval-gate policy.
- Validation scripts to ensure the template and project are safe to modify.

## Notes

This persona models Codex itself as a participant in the delivery process. Understanding its perspective helps ensure that the template provides the right scaffolding and instructions for successful autonomous operation.
