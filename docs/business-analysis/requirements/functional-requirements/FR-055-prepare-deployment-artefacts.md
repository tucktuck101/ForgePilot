# FR-055: Prepare deployment artefacts

## Document Metadata

| Field | Value |
|---|---|
| Document type | Functional Requirement |
| Status | Draft |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Linked artefacts | [index](index.md) |
| Update rule | Update when this requirement changes materially |

## Summary

The system shall prepare deployment artefacts when required, such as Dockerfiles, Docker Compose files, GitHub Actions workflows, environment variable documentation, deployment instructions, smoke test scripts, and rollback notes.

## Details

As part of deployment preparation, Codex should create or update configuration files needed to deploy the prototype to local, CI, or cloud environments. This may include containerisation (Dockerfiles and Compose files), environment variable documentation, CI/CD workflows, and smoke tests to verify that the deployed application works. Deployment instructions should be included in the handoff package, and any required secrets should be documented in `docs/solution-design/secrets-and-config.md`.

## Acceptance Criteria

- Deployment artefacts are created or updated when the project requires deployment.
- Deployment instructions specify how to build, run, and test the deployed prototype.
- Environment variables are documented in `docs/solution-design/secrets-and-config.md`.
- Smoke test scripts exist to verify basic functionality after deployment.
- Rollback notes are provided where appropriate.

## Notes

Preparing deployment artefacts helps ensure that ForgePilot prototypes can be run and tested consistently in different environments.
