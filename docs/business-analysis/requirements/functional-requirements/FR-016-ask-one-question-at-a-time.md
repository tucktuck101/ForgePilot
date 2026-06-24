# FR-016: Ask one question at a time

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

During the discovery interview, Codex shall ask the user one focused question at a time instead of presenting multiple questions in a single prompt. This helps prevent cognitive overload and ensures the user can provide thoughtful answers.

## Details

- The discovery process should be broken into discrete questions covering the product goal, users, problem, hypothesis, scope, and acceptance criteria.
- Codex should wait for an answer before asking the next question.
- Each question should be clear, concise, and limited in scope.
- If a question leads to a dependency on previous answers, Codex should reference the relevant information to avoid repetition.

## Acceptance Criteria

- Users receive one question per message from Codex during discovery.
- Codex does not combine multiple topics into a single question.
- Responses are captured and used to formulate subsequent questions or documents.

## Notes

This requirement ensures user comfort and engagement while collecting sufficient information, supporting FR-015 (chat-driven discovery).
