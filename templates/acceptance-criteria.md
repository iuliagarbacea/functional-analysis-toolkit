# Acceptance criteria: US-000

> One criterion, one observable outcome, one verdict (pass/fail). If you cannot say how you would check it, it is a wish, not a criterion.

**Story:** US-000
**Status:** Draft | Agreed | Verified
**Agreed with:** — on YYYY-MM-DD

## Criteria

### AC-000-1: [short name]

```gherkin
Given  [the precondition, including the role and the data state]
When   [one action]
Then   [one observable result]
And    [another observable result, only if it belongs to the same action]
```

**How verified:** manual / scripted / both · **Test cases:** TC-000-1
**Notes:** edge values, the exact message text, the exact field, the exact permission.

### AC-000-2: [short name]

```gherkin
Given  …
When   …
Then   …
```

## Negative and edge criteria

At least one criterion for each of: invalid input, missing permission, empty state, boundary value, concurrent change (if relevant). A story with only happy-path criteria is not Agreed.

## Explicitly not covered

What a reader might expect to find here and will not, with the reason.

## Checklist before marking Agreed

- [ ] Every criterion has exactly one *When*.
- [ ] Every *Then* names something a tester can see, read or query.
- [ ] Every business rule in the story maps to at least one criterion.
- [ ] Message texts, field labels and states are quoted exactly as they will appear.
- [ ] The business owner has read these, not just the story.
