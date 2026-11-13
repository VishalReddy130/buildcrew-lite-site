# BuildCrew handoff — INV-003

Project: Inventory API
Task: Implement low-stock endpoint
Owner role: developer
Priority: P0

## Context
Return items whose current quantity is at or below their reorder threshold.

## Acceptance criteria
- Items at the threshold are included.
- Items above the threshold are excluded.
- A missing item list returns an empty list.

## Guardrails
Inspect the repository first. Work only on this task. Do not invent test results. Do not mark the task done; human review is required.
