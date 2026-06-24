# FR-061: Document required secrets

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

The system shall document required secrets and configuration in `docs/solution-design/secrets-and-config.md`.

## Details

For each project, Codex should identify and document any secrets, API keys, tokens, or credentials that are needed to run, test, or deploy the application. This documentation should list environment variable names, descriptions, and whether they are required or optional. It should not include the actual secret values. The file should also describe any configuration keys that are not secrets but are necessary for the application to function.

## Acceptance Criteria

- A `docs/solution-design/secrets-and-config.md` file exists in the repository.
- The file lists all required environment variables and secrets with descriptions and indicates whether each is required or optional.
- The file does not include actual secret values—only names and descriptions.
- The documentation is referenced from other artefacts where relevant, such as deployment instructions and setup guides.

## Notes

Clear documentation of required secrets helps users and maintainers set up and deploy ForgePilot projects without exposing sensitive information.
