# US-034: Validate the ForgePilot Factory

## Document Metadata

| Field | Value |
|---|---|
| Object ID | US-034 |
| Document type | User Story |
| Status | Draft |
| Priority | Must |
| Owner/audience | Repo Bootstrapper, Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-006](../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Evidence | [EVD-001](../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | [User Stories Index](index.md) |
| Related objects | [User Stories Index](index.md), [SN-006](../discovery/stakeholder-needs/SN-006-repeatable-quality-validation.md) |
| Update rule | Update when this user story changes materially |

## Summary

Capture the Repo Bootstrapper need to validate the ForgePilot template.

## Story

As a Repo Bootstrapper, I want the template itself to be validated so that broken skills, templates, docs, or scripts are caught early.

## Acceptance Criteria

- Factory validation script exists.
- GitHub Actions workflow runs factory validation.
- Required files/folders are checked.
- Examples are clearly marked.
- Secret scanning checks are included where practical.

## Notes

None.
