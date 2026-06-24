# FR-033: Use small sprints for risky work

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | ../../index.md |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall encourage Codex to create small, focused sprints when tasks involve high uncertainty, risk, unfamiliar files, failing tests, sensitive data, or potential approval gates.

## Details

Situations warranting small sprints include:

- New codebases where Codex lacks context.
- Security, authentication, or data handling features.
- Complex integrations or external services.
- Changes spanning many files or components.
- Tasks requiring human approval before continuing.

Small sprints reduce the risk of wasted effort and make it easier to address unforeseen issues without overspending tokens.

## Acceptance Criteria

- Risky or ambiguous tasks are scoped into small sprints.
- Small sprints are documented with clear goals and boundaries.
- The logic for scoping small sprints is recorded in planning notes.

## Notes

This requirement complements FR-032 (adaptively selecting sprint scope) and helps maintain safe, incremental progress.
