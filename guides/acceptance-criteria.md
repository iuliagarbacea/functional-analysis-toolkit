# Writing acceptance criteria a tester can use

An acceptance criterion is a check. Not a hope, not a description, not a reminder. A tester reads it, does something, observes something, and says pass or fail. If any of those three steps is unclear, the criterion is not finished.

## The test for a criterion

Ask: *if two testers who have never met ran this, would they reach the same verdict?*

- "The form should be user friendly" fails the test. Two testers, two opinions.
- "The form validates input" fails the test. Which input, which rule, what happens?
- "Given an editor on the case form, when they submit with the *Case title* field empty, then the form is not submitted and the message *Case title is required* appears under the field" passes. Anyone can run it.

## Given / When / Then, used properly

**Given** is the state of the world before the action: the role, the data, the page, the flags. Everything the tester needs to set up. If they have to guess how to get there, the Given is incomplete.

**When** is one action. One. "When they submit" is a criterion. "When they fill in the form and submit and then go to the list" is three criteria pretending to be one, and when it fails nobody knows which part broke.

**Then** is what can be observed. A message text, quoted exactly. A field state. A record in a table. A status code. An email received. "Then it works" is not a Then.

## Where criteria usually fall short

- **Only the happy path.** Every story needs at least: invalid input, missing permission, empty state, boundary value. If concurrency matters, that too. A story with only happy-path criteria is not ready for build.
- **Texts paraphrased.** "An error message appears" versus "the message *Case title is required* appears". The second one catches the typo, the wrong field, the wrong language.
- **Rules without criteria.** Every business rule in the story should map to at least one criterion. Walk the rules list and check.
- **Criteria without an owner's eyes.** The business owner has read the story. Did they read the criteria? The criteria are what the team will actually build. The story is what they will remember asking for. Those two drift.

## Criteria and test cases are not the same thing

The criterion says what must be true. The [test case](../templates/test-case.md) says how to check it on a specific environment with specific data, step by step. One criterion often needs several test cases: one per boundary, one per role. Keep them separate and link them by ID. When the environment changes, the test cases change and the criteria do not.

## A short checklist

- [ ] Exactly one *When* per criterion.
- [ ] Every *Then* is observable.
- [ ] Texts, labels and states quoted exactly.
- [ ] Negative and edge cases present.
- [ ] Every business rule covered.
- [ ] Business owner has read the criteria, not just the story.
