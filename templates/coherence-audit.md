# Coherence audit: [project], YYYY-MM-DD

> A document set drifts. Numbers get updated in one file and not another; a decision is reversed but two documents still assume it. This audit finds the drift before a reader or an auditor does.

**Audited set:** [document + version, one per line]
**Auditor:** — · **Duration:** —
**Previous audit:** YYYY-MM-DD · **Findings then:** n · **Still open:** n

## Method

1. List every **fact that appears in more than one document**: totals, percentages, dates, names, counts, IDs. These are the audit candidates.
2. For each, record the value in each document. Any mismatch is a finding.
3. For every **decision ID referenced**, check the register: is it Active? Does the citing text match the decision as recorded?
4. For every **cross-reference** (document + version + section), check that the target version is current and the section still exists and still says what the citation claims.
5. Check **status fields**: anything marked Draft that is cited as final, anything Superseded still in the working folder.

## Findings

| # | Fact / reference | Doc A says | Doc B says | Source of truth | Fix | Owner | Fixed on |
|---|---|---|---|---|---|---|---|
| 1 | Total budget | 694 500 (Req v4 §1) | 690 000 (Plan v3 §2) | Register D-022 | Plan v3 to v4 | | |

## Summary

| | Count |
|---|---|
| Facts checked | |
| Mismatches | |
| Stale decision references | |
| Broken cross-references | |
| Status inconsistencies | |

## Root causes noted

One line each. The point is to change the process, not just the number.
