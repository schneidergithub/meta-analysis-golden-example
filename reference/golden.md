# Golden reference

This analysis follows the [Golden example 1 calculation card](../studies.md#golden-example-1-calculation-card). Keep this reference outside the inputs supplied during an attempt.

## Evidence

Each school reports 50 students per group and a sample standard deviation of 10 in both groups. Each difference is the practice-question group's average exam score minus the rereading group's average exam score.

| School | Source | Practice-question group average | Rereading group average | Difference in exam points |
| --- | --- | ---: | ---: | ---: |
| Oak | Table O1 | 76 | 70 | 6 |
| Pine | Table P1 | 74 | 70 | 4 |
| Maple | Table M1 | 78 | 70 | 8 |

## Analysis

### 1. Calculate each school's result

The differences are 6 points for Oak, 4 for Pine, and 8 for Maple.

For each school, calculate:

- Each group's contribution to the variance: (10 × 10) ÷ 50 = 2
- **Variance:** 2 + 2 = 4
- **Weight:** 1 ÷ 4 = 0.25

### 2. Combine the schools

- **Total weight:** 0.25 + 0.25 + 0.25 = 0.75
- **Total of the three products:** (6 × 0.25) + (4 × 0.25) + (8 × 0.25) = 4.5
- **Combined difference:** 4.5 ÷ 0.75 = 6 points

### 3. Calculate the uncertainty

- **Standard error:** square root of (1 ÷ 0.75)
- **Margin:** 1.96 × square root of (1 ÷ 0.75)
- **Lower limit:** 6 − margin, approximately 3.74 points
- **Upper limit:** 6 + margin, approximately 8.26 points

The combined difference is **6 points**, with an approximate **95% confidence interval of 3.74 to 8.26 points**. The interval limits are rounded here for display.

## Interpretation

Across the three schools, the practice-question groups scored an estimated 6 points higher on average than the rereading groups. The interval describes uncertainty in the combined difference under the calculation card's assumptions. It does not describe individual students' scores. These fictional results do not establish effectiveness in real schools.

## Review

Check the source values and calculation steps as well as the final result. Equal weights make the combined estimate equal to a simple average, so an answer of 6 alone is insufficient.

Accept equivalent arithmetic and explanations in the assignee's own words. Record missing work, calculation errors, and departures from the specified method separately.
