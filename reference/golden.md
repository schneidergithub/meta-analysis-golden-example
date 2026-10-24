# Worked answer

This analysis follows the [calculation card](../studies.md#calculation-card). Keep this worked answer out of the materials supplied during an attempt.

See the [shared glossary](../glossary.md) for explanations of the terms used below.

## Evidence

Each school reports 50 students per group and a [sample](../glossary.md#sample) [standard deviation](../glossary.md#standard-deviation) of 10 in both groups. Each [school's estimated difference](../glossary.md#schools-estimated-difference) is the practice-question group's [average score](../glossary.md#average-score) minus the rereading group's average score.

| School | Source | Practice-question group average score | Rereading group average score | School's estimated difference in exam points |
| --- | --- | ---: | ---: | ---: |
| Oak | Table O1 | 76 | 70 | 6 |
| Pine | Table P1 | 74 | 70 | 4 |
| Maple | Table M1 | 78 | 70 | 8 |

## Analysis

### 1. Calculate each school's result

The estimated differences are 6 points for Oak, 4 for Pine, and 8 for Maple.

For each school, calculate:

- Each group's contribution to the variance of the estimated difference: (10 × 10) ÷ 50 = 2
- **[Variance of the estimated difference](../glossary.md#variance-of-the-estimated-difference):** 2 + 2 = 4
- **[Weight](../glossary.md#weight):** 1 ÷ 4 = 0.25

### 2. Combine the schools

- **[Total weight](../glossary.md#total-weight):** 0.25 + 0.25 + 0.25 = 0.75
- **[Weighted differences](../glossary.md#weighted-difference):** Oak: 6 × 0.25 = 1.5; Pine: 4 × 0.25 = 1; Maple: 8 × 0.25 = 2
- **Sum of the weighted differences:** 1.5 + 1 + 2 = 4.5
- **[Combined difference](../glossary.md#combined-difference):** 4.5 ÷ 0.75 = 6 points

### 3. Calculate the uncertainty

- **[Standard error](../glossary.md#standard-error):** square root of (1 ÷ 0.75)
- **[Margin](../glossary.md#margin):** 1.96 × square root of (1 ÷ 0.75)
- **Lower limit:** 6 − margin, approximately 3.74 points
- **Upper limit:** 6 + margin, approximately 8.26 points

The combined difference is **6 points**, with an approximate **[95% confidence interval](../glossary.md#95-confidence-interval) of 3.74 to 8.26 points**. The interval limits are rounded here for display.

## Interpretation

Across the three schools, the practice-question groups scored an estimated 6 points higher on average than the rereading groups. The interval describes uncertainty in the combined difference under the calculation card's assumptions. It does not describe individual students' scores. These fictional results do not establish effectiveness in real schools.

## Review

Check the steps as well as the answer: several shortcuts also produce 6. Here, equal weights make the combined estimate equal to a simple average.

Accept equivalent arithmetic and explanations in the participant's own words. Record missing work, calculation errors, and use of a different calculation method separately.
