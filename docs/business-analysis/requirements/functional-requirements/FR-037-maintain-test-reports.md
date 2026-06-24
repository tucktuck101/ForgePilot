# FR-037: Maintain test reports

## Document Metadata

| Field | Value |
|---|---|
| Object ID | FR-037 |
| Document type | Functional Requirement |
| Status | Draft |
| Priority | Must |
| Owner/audience | Product Owner, Codex, future maintainers |
| Source | ForgePilot business analysis conversation |
| Source need(s) | [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Evidence | [EVD-001](../../discovery/evidence/EVD-001-stakeholder-request-2026-06-24.md), [EVD-002](../../discovery/evidence/EVD-002-existing-business-analysis-corpus.md) |
| Linked artefacts | ../../index.md |
| Related objects | ../../index.md, [SN-005](../../discovery/stakeholder-needs/SN-005-traceable-delivery-and-decisions.md) |
| Update rule | Update when this functional requirement changes materially |

## Summary

ForgePilot shall collect and store test results in a central location, such as `docs/business-analysis/delivery/test-reports.md`, for each sprint or major work item.

## Details

- After running tests during each sprint, Codex should summarise the results in a test report file.
- The report should include which tests were run, pass/fail outcomes, and any noteworthy issues.
- If tests fail due to unrelated problems, those should be documented separately to avoid confusion.
- The test report file should be appended or updated per sprint, linking to the corresponding sprint notes.

## Acceptance Criteria

- A `test-reports.md` file exists under `docs/business-analysis/delivery/`.
- Test results are recorded after each sprint.
- Pass/fail status and relevant details are included for all tests executed.

## Notes

Maintaining test reports helps track the stability of the codebase over time and provides evidence of quality when handing off the prototype.
