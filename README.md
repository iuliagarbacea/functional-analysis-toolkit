# Functional Analysis Toolkit

Templates and short guides for functional analysis and testing work. These are the documents I use on real projects, stripped of client content. Nothing here is theory: every template exists because a missing one once cost a team a week.

Written in Markdown so they live next to the code, diff cleanly, and survive tool changes. Copy, adapt, keep what earns its place.

## Templates

| Template | Use it when |
|---|---|
| [user-story.md](templates/user-story.md) | Turning a request into a unit of work a developer can estimate |
| [acceptance-criteria.md](templates/acceptance-criteria.md) | Deciding, before the build, what "done" will be checked against |
| [requirements-traceability-matrix.md](templates/requirements-traceability-matrix.md) | Proving every requirement has a test and every test has a reason |
| [test-case.md](templates/test-case.md) | Writing one check so that someone else can run it identically |
| [test-register.csv](templates/test-register.csv) | Tracking the whole set of checks across runs and environments |
| [defect-report.md](templates/defect-report.md) | Reporting a failure so it gets fixed the first time |
| [decision-register.md](templates/decision-register.md) | Recording decisions with IDs that are never reused |
| [document-control.md](templates/document-control.md) | Versioning a document set and archiving superseded versions |
| [coherence-audit.md](templates/coherence-audit.md) | Checking that a set of documents still agrees with itself |
| [uat-signoff.md](templates/uat-signoff.md) | Closing a delivery with a signature that means something |

## Guides

- [Running a decision register](guides/decision-register.md): the three rules that make it work
- [Auditing a document set for coherence](guides/coherence-audit.md): how drift happens and how to find it in an afternoon
- [Writing acceptance criteria a tester can use](guides/acceptance-criteria.md): the difference between a wish and a check

## Principles behind the templates

1. **One source of truth per fact.** A number, a date, a name lives in exactly one place. Everything else references it.
2. **IDs are never reused.** A retired ID stays retired. If D-031 is superseded, the replacement is D-032, not D-031 v2.
3. **Superseded is not deleted.** Old versions move to an archive folder with the date they were superseded. History stays auditable.
4. **A check that cannot be written down is not a check.** If two people would run it differently, the test case is not finished.
5. **Audit the set, not the document.** Documents drift apart from each other, not from themselves.

## Licence

[CC BY 4.0](LICENSE). Use them, change them, credit the source.
