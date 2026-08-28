# Metadata — Descriptive-Statistics/Sample-Mean/question.xml

Running record of every agent (and user) action on this question that
isn't the XML itself: the reasoning, findings, improvement notes, and
reference lookups behind each change. Entries are appended in order,
newest at the bottom. The XML changes themselves are recorded by git —
this file holds the substance and meaning behind them, not the diffs.

## Entry 1 — concierge (2026-08-28T11:59:36)

**Issue:**
- #4

**Closes on merge:**
- yes

**Reference files fetched:**
- (none)

```text
Question reserved as part of issue #4.
```

## Entry 2 — planner (2026-08-28T12:02:15)

**Reference files fetched:**
- (none)

**Reference files recommended by Planner:**
- Authoring/Answer_Tests/Grading_recipes.md

```text
GOAL (non-negotiable): Test whether the student can correctly compute the sample mean (arithmetic average) of a small dataset — sum divided by count.

STRUCTURE (non-negotiable): Single-part question. Student is shown 6 randomized integer data values and enters one numeric answer: the sample mean, as a decimal.

RANDOMIZATION (negotiable unless stated otherwise below): The 6 data values are integers independently randomized in range 1–30, inclusive, with repeats allowed (no distinctness constraint).

ANSWER TESTS (negotiable unless stated otherwise below): Numeric input; the student's answer is checked against the true mean with a numerical tolerance of about ±0.01 to absorb rounding to 2 decimal places. Exact decimal-place formatting is not strictly enforced — an answer equivalent within tolerance (e.g. 15 vs 15.00) is accepted as correct.

FEEDBACK (negotiable unless stated otherwise below):
- Correct: brief reminder of the formula — sample mean = (sum of values) ÷ (number of values) — as reinforcement, not as new information.
- Incorrect: a hint to recheck their addition of the six values and confirm they divided by the correct count (6), without revealing the actual mean or any intermediate computed value.

PRT/QTEST SUGGESTIONS: (none)
```

