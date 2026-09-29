# Decision register: [project]

> The register is the single place where decisions live. If it is not here, it was not decided.

**Current revision:** rev. 1 · **Date:** YYYY-MM-DD · **Owner:** —

## Rules

1. IDs are sequential and **never reused**. A superseded or reversed decision keeps its ID and its row.
2. Every decision records who made it and on what date. "The team" is not a who.
3. A decision that changes another one names it: *Supersedes D-012*. The old row gets *Superseded by D-031*.
4. The register has a revision number. Any change to any row bumps it and is noted in the revision log.
5. Other documents reference decisions by ID. They never restate them.

## Register

| ID | Date | Decision | Rationale (short) | Decided by | Status | Supersedes / superseded by | Affects |
|---|---|---|---|---|---|---|---|
| D-001 | YYYY-MM-DD | One sentence, stated as the thing that will now be true | Why, in one or two sentences | Name, role | Active | — | US-003, doc X §2 |
| D-002 | YYYY-MM-DD | | | | Superseded | by D-007 | |
| D-003 | YYYY-MM-DD | | | | Reversed | — | |

**Status values:** Proposed · Active · Superseded · Reversed · Cancelled

## Open decisions

| ID | Question | Options considered | Needed by | Blocking |
|---|---|---|---|---|
| D-004 | | | YYYY-MM-DD | US-009 |

## Revision log

| Rev. | Date | Change | By |
|---|---|---|---|
| 1 | YYYY-MM-DD | Register created | |
