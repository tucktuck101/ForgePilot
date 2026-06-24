# FR-019: Request product brief approval

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

ForgePilot shall require human approval of the product brief before moving into solution design. The product brief summarises the app idea, target users, problem statement, prototype hypothesis, scope, success criteria, assumptions, and constraints.

## Details

After the discovery artefacts are drafted, Codex should:

- Present the product brief to the user for review.
- Explain that this document defines what the project will aim to achieve.
- Request explicit approval to proceed with solution design.
- Record the approval decision and, if necessary, any revisions requested by the user.

No architectural or development work should begin until this approval is obtained.

## Acceptance Criteria

- Codex asks for approval of the product brief.
- Approval status (approved/rejected/revisions needed) is captured.
- If approved, solution design can begin.
- If revisions are required, the brief is updated and approval is requested again.

## Notes

This requirement aligns with the approval gate policy to ensure the project direction is validated by the user.
