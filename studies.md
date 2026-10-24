# Supplied studies

These are fictional studies created for this exercise.

## Shared study conditions

The experiment compares 2 different groups of students, from 3 different schools: 
-  One group of students used practice questions to prepare for a test.
-  The other group prepared for the test by rereading their notes instead. 

Both groups started with the same course materials. Students studied for the same amount of time over six weeks, then took the same exam.

Within each school, 100 students were randomly assigned, 50 to practice questions and 50 to rereading notes.

The tables report group averages and sample standard deviations.

## Golden example 1 calculation card

This example measures whether you can extract the evidence and reproduce an analysis.



For each school, calculate:

- `difference = practice_mean - rereading_mean`
- `variance = (practice_standard_deviation * practice_standard_deviation) / practice_student_count + (rereading_standard_deviation * rereading_standard_deviation) / rereading_student_count`
- `weight = 1 / variance`

Then combine the three schools:

- `total_weight = sum of the three weights`
- `combined_difference = sum of (weight * difference) for the three schools / total_weight`
- `combined_standard_error = square root of (1 / total_weight)`
- `lower_limit = combined_difference - 1.96 * combined_standard_error`
- `upper_limit = combined_difference + 1.96 * combined_standard_error`

The lower and upper limits form the approximate 95% confidence interval. Use exactly `1.96` as the multiplier. This is a common-effect inverse-variance analysis: for this exercise, assume the studies estimate a common underlying effect and treat the groups and studies as independent. 

Show the extracted numbers and their source tables, each school's difference, variance and weight, and the combined result and confidence interval. Explain the finding and uncertainty in your own words.

## Oak School

**Table O1. Oak School exam results after six weeks**

| Study method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 76 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Pine School

**Table P1. Pine School exam results**

| Study method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 74 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Maple School

**Table M1. Maple School exam results**

| Study method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 78 | 10 |
| Rereading notes | 50 | 70 | 10 |
