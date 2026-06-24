# FR-056: Require pre-deployment approval

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

The system shall require human approval before deploying any prototype to an externally accessible environment.

## Details

Deployment of prototypes should be treated as a critical approval gate. Codex must prepare deployment artefacts and instructions but must not deploy publicly accessible versions without explicit approval from the user. Private, local, or staging deployments may be executed after approval if appropriate. Deployment approval requests should clearly explain the target environment, expected endpoints, and any associated costs, security implications, or risks.

## Acceptance Criteria

- Deployment preparation stops and requests approval before any public or external deployment.
- The approval request clearly describes what will be deployed, where it will run, and any potential costs or risks.
- Codex waits for explicit approval before executing deployment to external environments.
- Deployment to local or private staging environments is allowed after approval, if appropriate.

## Notes

Requiring pre-deployment approval protects users from unintended exposure or costs and maintains control over release timing.
