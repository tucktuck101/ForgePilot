# FR-041: Create draft pull requests

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

At the start of each sprint, ForgePilot should create a draft pull request (PR) that tracks the changes made during the sprint. This PR will be updated with new commits and information as the sprint progresses.

## Details

- The draft PR should be opened immediately after creating the sprint branch.
- The PR title should reflect the sprint goal or associated issue.
- The PR description should summarise the scope of the sprint and link to the issue.
- Codex updates the PR description with test results, risks, and other relevant information as work progresses.
- The PR remains in draft state until the sprint’s definition of done is satisfied.

## Acceptance Criteria

- A draft PR is created at the start of each sprint.
- The PR is linked to its corresponding issue.
- The PR remains draft until ready for review.
- All necessary details are updated before marking it ready for review.

## Notes

This requirement aligns with the one PR per sprint rule and supports transparency and incremental review during development.
