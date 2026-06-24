# FR-078: Include Setup, Run, Test, and Deployment Information

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [Functional Requirements Index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The final handoff document must include setup, run, test, and deployment instructions.

## Details

A handoff is not complete without clear instructions for using the delivered prototype. The final handoff document must provide:

- Setup instructions (dependencies, environment variables, local setup commands)
- Run instructions (how to start the application locally and any recommended environment settings)
- Test instructions (commands to run tests and interpret results)
- Deployment instructions or the staging URL if deployment has been approved, including required environment variables, secrets, and smoke tests

These sections ensure that future users can evaluate and operate the prototype without guesswork.

## Acceptance Criteria

- The final handoff includes clearly labelled sections for setup, run, test, and deployment instructions or staging URL.
- Required environment variables and secrets are referenced and documented (but not included) appropriately.
- Commands are presented in a format suitable for copy-pasting into a terminal.

## Notes

This requirement ensures that prototypes are usable and deployable by reviewers and future maintainers.
