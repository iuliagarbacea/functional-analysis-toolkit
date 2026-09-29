# Requirements traceability matrix: [project / release]

> Purpose: prove that every requirement is covered by at least one test, and that every test exists for a reason. Rows with an empty cell are the finding.

**Version:** 1.0 · **Date:** YYYY-MM-DD · **Owner:** —
**Source documents:** [requirements doc + version], [test register + version]

| Requirement ID | Requirement (short) | Source | Story | Acceptance criteria | Test cases | Last run | Result | Gap / note |
|---|---|---|---|---|---|---|---|---|
| REQ-001 | | | US-001 | AC-001-1, AC-001-2 | TC-001-1, TC-001-2 | YYYY-MM-DD | Pass | |
| REQ-002 | | | US-002 | AC-002-1 | — | — | — | **No test case** |
| — | | | US-003 | AC-003-1 | TC-003-1 | | | **Test without requirement** |

## Coverage summary

| | Count |
|---|---|
| Requirements | |
| Requirements with at least one test | |
| Requirements with no test | |
| Tests with no requirement | |
| Tests not run this cycle | |

## Rules

1. The matrix is regenerated, not hand-edited, wherever the source data allows. If it is hand-edited, record the date and the source document versions above.
2. A requirement counts as covered only when the linked test has run against the current build and passed.
3. Orphan tests are either linked to a requirement, or the requirement is written, or the test is retired. Never left as is.
