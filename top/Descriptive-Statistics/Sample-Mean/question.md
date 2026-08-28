# Metadata — Descriptive-Statistics/Sample-Mean/question.xml

Running record of every agent (and user) action on this question that
isn't the XML itself: the reasoning, findings, improvement notes, and
reference lookups behind each change. Entries are appended in order,
newest at the bottom. The XML changes themselves are recorded by git —
this file holds the substance and meaning behind them, not the diffs.

## Entry 1 — concierge (2026-08-28T11:58:15)

**Issue:**
- #2

**Closes on merge:**
- yes

**Reference files fetched:**
- (none)

```text
Question reserved as part of issue #2.
```

## Entry 2 — planner (2026-08-28T12:04:44)

**Reference files fetched:**
- (none)

**Reference files recommended by Planner:**
- Authoring/Answer_Tests/Grading_recipes.md

```text
GOAL (non-negotiable): Test whether the student can compute the arithmetic mean of a small raw dataset — routine calculation, checking accurate summation and division by the correct count.

STRUCTURE (non-negotiable): Single-part. The question presents 6 randomized integer data values; the student enters a single numeric value for the sample mean.

RANDOMIZATION (negotiable unless stated otherwise below): Six integers, each independently drawn from roughly 1 to 30 inclusive, with repeats allowed (no distinctness constraint). No further constraint on their sum or resulting mean (a non-terminating decimal mean is fine and arguably better, since it tests real division rather than eyeballing).

ANSWER TESTS (negotiable unless stated otherwise below): Numerical input, a single decimal number. Graded as correct if within absolute tolerance of about 0.01 of the true mean (sum of the six values divided by 6). Any number of decimal places accepted from the student — no format/precision requirement enforced.

FEEDBACK (negotiable unless stated otherwise below): 
- Correct: briefly restate the method — mean = (sum of values) ÷ (count of values) — with the actual sum and count substituted in, confirming the value.
- Incorrect: a general hint prompting the student to recheck their sum and their count of values, without revealing the correct mean or doing the arithmetic for them.

PRT/QTEST SUGGESTIONS: (none)
```

