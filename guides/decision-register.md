# Running a decision register

A decision register is a table. What makes it work is not the table, it is three rules that most teams break within a month.

## Rule 1: an ID is never reused

When decision D-031 is overturned, the new decision is D-032. D-031 stays in the register with status *Superseded by D-032*.

Why it matters: six months later someone finds "per D-031" in an old email or a specification. If D-031 still means what it meant when that text was written, the reference is still true and the reader can follow the trail to D-032. If D-031 has quietly been rewritten, every document that cited it is now silently wrong and nobody knows which ones.

Reusing an ID feels tidy. It destroys the audit trail.

## Rule 2: the register has a revision number, and every change bumps it

Not just new rows. Any edit to any cell. Rev. 26 means "this register has been changed 26 times", and the revision log says what changed when.

Why it matters: other documents cite "register rev. 19". When the register is at rev. 26, you know those documents were written against an older state and need a coherence check. Without the revision number, you cannot tell whether a document is stale.

## Rule 3: decisions are referenced, never restated

A specification says "the retention period follows D-017". It does not say "the retention period is 5 years (D-017)". The number lives in one place, the register.

Why it matters: if the period changes to 7 years, one row changes. If the number was copied into eight documents, eight documents change, and in practice five of them do. The [coherence audit](../templates/coherence-audit.md) exists to find the other three, but not copying the number is cheaper than auditing it.

## What a decision row needs

- **One sentence, stated as what is now true.** "Suppliers are paid at 30 days" beats "we discussed payment terms and leaned toward 30 days".
- **Who decided, by name and role.** "The team" or "the workshop" is not an owner. When the decision is questioned, someone has to be able to say why.
- **The rationale, short.** Two sentences. Enough that the next person does not reopen the question from zero.
- **What it affects.** Story IDs, document sections. This is what makes the coherence audit possible.

## Open decisions belong in the register too

A question that blocks work is a decision waiting to happen. Give it an ID now, with status *Proposed*, a "needed by" date, and the thing it blocks. When it is answered, the row changes status. If it is answered outside the register and nobody writes it down, rule 3 has just been broken.

## When the register is the deliverable

On regulatory or funded projects the register is not a working aid, it is evidence. In that case: keep it in a format that shows history (a versioned file, not a live wiki page), export a dated copy at every milestone, and make the revision log part of the document. An auditor who can trace D-001 to D-109 without asking a question is an auditor who leaves early.
