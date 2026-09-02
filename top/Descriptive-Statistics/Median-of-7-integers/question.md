# Metadata — Descriptive-Statistics/Median-of-7-integers/question.xml

Running record of every agent (and user) action on this question that
isn't the XML itself: the reasoning, findings, improvement notes, and
reference lookups behind each change. Entries are appended in order,
newest at the bottom. The XML changes themselves are recorded by git —
this file holds the substance and meaning behind them, not the diffs.

## Entry 1 — concierge (2026-09-02T17:37:12)

**Issue:**
- #8

**Closes on merge:**
- yes

**Reference files fetched:**
- (none)

```text
Question reserved as part of issue #8.
```

## Entry 2 — planner (2026-09-02T17:38:50)

**Reference files fetched:**
- (none)

**Reference files recommended by Planner:**
- Authoring/Answer_Tests/Grading_recipes.md

```text
GOAL (non-negotiable): Test whether a student can correctly compute the median of a set of 7 integers by requiring them to sort the values and identify the middle one.

STRUCTURE (non-negotiable): Single-part question. One numeric input for the median value, graded by one PRT.

RANDOMIZATION (negotiable unless stated otherwise below): Seven integers, each independently randomized in the range 1–50 inclusive, repeats allowed. Displayed to the student in random (unsorted, shuffled) order. Guard against the degenerate case where all 7 values are identical (regenerate if so, so the exercise isn't trivial).

ANSWER TESTS (negotiable unless stated otherwise below): Single numeric input, integer type. Correct answer is the exact integer median (the 4th value once the 7 are sorted ascending). Exact match required — no tolerance.

FEEDBACK (negotiable unless stated otherwise below):
- Correct: brief explanation of the method — sort the 7 values into order, then take the middle (4th) value.
- Incorrect, generic: hint to double-check they sorted the values first before picking the middle one; does not reveal the actual median.
- Incorrect, specific branch 1: if the student's answer equals the middle value of the *unsorted* (as-displayed) list, give feedback pointing out that the values need to be sorted first, not read off in the order shown.
- Incorrect, specific branch 2: if the student's answer equals the mean of the 7 values (rounded to the nearest integer, to allow for a non-integer mean), give feedback clarifying that the median is the middle value after sorting, not the average.
- Any other incorrect answer: falls to the generic incorrect feedback above.

PRT/QTEST SUGGESTIONS: (none)
```

## Entry 3 — planner (2026-09-02T17:40:15)

**Reference files fetched:**
- (none)

**Reference files recommended by Planner:**
- Authoring/Answer_Tests/Grading_recipes.md

```text
GOAL (non-negotiable): Test whether a student can correctly compute the median of a set of 7 integers by requiring them to sort the values and identify the middle one.

STRUCTURE (non-negotiable): Single-part question. One numeric input for the median value, graded by one PRT.

RANDOMIZATION (negotiable unless stated otherwise below): Seven integers, each independently randomized in the range 1–50 inclusive, repeats allowed. Displayed to the student in random (unsorted, shuffled) order. Guard against the degenerate case where all 7 values are identical (regenerate if so, so the exercise isn't trivial).

ANSWER TESTS (negotiable unless stated otherwise below): Single numeric input, integer type. Correct answer is the exact integer median (the 4th value once the 7 are sorted ascending). Exact match required — no tolerance.

FEEDBACK (negotiable unless stated otherwise below):
- Correct: brief explanation of the method — sort the 7 values into order, then take the middle (4th) value.
- Incorrect, generic: hint to double-check they sorted the values first before picking the middle one; does not reveal the actual median.
- Incorrect, specific branch 1: if the student's answer equals the middle value of the *unsorted* (as-displayed) list, give feedback pointing out that the values need to be sorted first, not read off in the order shown.
- Incorrect, specific branch 2: if the student's answer equals the mean of the 7 values (rounded to the nearest integer, to allow for a non-integer mean), give feedback clarifying that the median is the middle value after sorting, not the average.
- Any other incorrect answer: falls to the generic incorrect feedback above.

PRT/QTEST SUGGESTIONS: (none)
```

