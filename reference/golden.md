# Golden reference

This analysis follows the [Golden example 1 calculation card](../studies.md#golden-example-1-calculation-card). Keep this reference outside the inputs supplied during an attempt.

## Evidence

Each school reports 50 students per group and a sample standard deviation of 10 in both groups. Differences are practice minus rereading, in exam points.

| School | Source | Practice mean | Rereading mean | Difference |
| --- | --- | ---: | ---: | ---: |
| Oak | Table O1 | 76 | 70 | 6 |
| Pine | Table P1 | 74 | 70 | 4 |
| Maple | Table M1 | 78 | 70 | 8 |

## Analysis

For each school:

- `variance = (10 * 10) / 50 + (10 * 10) / 50 = 4`
- `weight = 1 / 4 = 0.25`

Combine the three schools:

- `total_weight = 0.25 + 0.25 + 0.25 = 0.75`
- `combined_difference = (0.25 * 6 + 0.25 * 4 + 0.25 * 8) / 0.75 = 6`
- `combined_standard_error = square root of (1 / 0.75)`
- `lower_limit = 6 - 1.96 * combined_standard_error`
- `upper_limit = 6 + 1.96 * combined_standard_error`

The combined difference is **6 points**, with an approximate **95% confidence interval of 3.74 to 8.26 points**. The interval limits are rounded here for display.

## Interpretation

The practice-question groups scored higher on average. The interval describes uncertainty in the combined difference under the calculation card's common-effect and independence assumptions. It does not describe individual students' scores. These fictional results do not establish effectiveness in real schools.

## Review

Check the source values and calculation steps as well as the final result. Equal weights make the combined estimate equal to a simple average, so an answer of 6 alone is insufficient.

Accept equivalent arithmetic and explanations in the assignee's own words. Record missing work, calculation errors, and departures from the specified method separately.
