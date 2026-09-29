# Auditing a document set for coherence

Documents rarely go wrong on their own. They go wrong relative to each other. The budget total is updated in the financial annex and not in the summary. A decision is reversed and two specifications still assume it. A percentage is recomputed and the old value survives in a footnote.

Nobody notices because everyone reads one document at a time. The reader who reads all of them is the auditor, the reviewer, or the client, and by then it is a finding against you.

## How drift happens

- **Copying instead of referencing.** The same number typed into four places. One gets updated.
- **Parallel editing.** Two people, two documents, one afternoon, no sync.
- **Late decisions.** Something changes in week 9 and the documents written in weeks 2 to 8 are never revisited.
- **Version confusion.** Someone edits v3 after v4 was issued, and the edit is lost or, worse, reintroduced.

## The audit, in an afternoon

1. **List the set.** Every document, with its current version. If you cannot state the current version of a document, that is finding number one.
2. **Extract the shared facts.** Go through each document and note every number, date, name, count and ID that could plausibly appear elsewhere. Totals, percentages, deadlines, headcounts, article numbers, decision IDs. Put them in a table with one column per document.
3. **Compare rows.** Any row with two different values is a finding. Record both values, both locations, and which one is the source of truth.
4. **Check decision references.** For every "per D-nnn", open the register. Is D-nnn still Active? Does the text that cites it still match what it says?
5. **Check cross-references.** For every "see document X, section Y", confirm X is the current version and section Y still exists and still says what the citation claims.
6. **Check statuses.** Anything Draft that is cited as final. Anything Superseded still sitting in the working folder.

Write findings in the [audit template](../templates/coherence-audit.md). Fix from the source of truth outward, then bump the versions of every document you touched.

## What a mature set looks like

- Shared facts are referenced, not copied. The audit table has mostly one value per row because the fact only lives in one place.
- Every document carries its version and the versions of the documents it depends on.
- Superseded versions are in a dated archive folder. Nothing is deleted, nothing old is in the working folder.
- The audit is run at every milestone and its findings count is trending to zero.

## The uncomfortable part

The first audit on a real project usually finds ten to twenty mismatches in a set that everyone believed was consistent. That is not a sign of a careless team. It is what happens to any document set edited by more than one person over more than one month. The audit is the process catching up with reality.
