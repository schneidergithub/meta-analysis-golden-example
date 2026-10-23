# Supplied studies

These are fictional studies created for this exercise. The schools, participants, and results are invented.

## Shared study conditions

Each school compared practice questions with rereading notes for the same course material. Students studied for the same amount of time over six weeks, then took the same exam, scored from 0 to 100. Higher scores mean better exam performance.

Within each school, 100 students were randomly assigned individually: 50 to practice questions and 50 to rereading notes. The groups contained different students, and no student took part in more than one school study. Everyone completed the exam. Each student contributed one final score.

The tables report group averages and sample standard deviations (SDs). The reported numbers are the supplied evidence; individual student scores are not provided.

## G01 calculation card

Use all three schools and the calculation rules below. This example measures whether you can extract the evidence and reproduce a specified analysis.

Measure each school's result in exam points: the practice-question average minus the rereading average. A positive result favors practice questions. In the formulas, `n` means the number of students, `SD` means the supplied sample standard deviation, `^2` means squared, and `sqrt` means square root.

For each school, calculate:

- `difference = practice_mean - rereading_mean`
- `variance = practice_SD^2 / practice_n + rereading_SD^2 / rereading_n`
- `weight = 1 / variance`

Then combine the three schools:

- `total_weight = sum of the three weights`
- `combined_difference = sum of (weight * difference) for the three schools / total_weight`
- `combined_standard_error = sqrt(1 / total_weight)`
- `lower_limit = combined_difference - 1.96 * combined_standard_error`
- `upper_limit = combined_difference + 1.96 * combined_standard_error`

The lower and upper limits form the approximate 95% confidence interval. Use exactly `1.96` as the multiplier. This is a common-effect inverse-variance analysis: for this exercise, assume the studies estimate a common underlying effect and treat the groups and studies as independent. Do not add a between-school variance term.

Keep full precision during calculations. Round reported school differences, the combined difference, and confidence interval limits to two decimal places.

Show the extracted numbers and their source tables, each school's difference, variance and weight, and the combined result and confidence interval. Explain the finding and uncertainty in your own words. For G01, use this specified analysis; any calculation approach that follows these formulas is acceptable.

## Oak School

Oak School compared the two methods using the shared study conditions above. Its results are reported in Table O1.

**Table O1. Oak School exam results after six weeks**

| Study method | Students | Average score | SD |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 76 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Pine School

Pine School conducted a separate study using the same conditions. Its results are reported in Table P1.

**Table P1. Pine School exam results after six weeks**

| Study method | Students | Average score | SD |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 74 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Maple School

Maple School conducted a separate study using the same conditions. Its results are reported in Table M1.

**Table M1. Maple School exam results after six weeks**

| Study method | Students | Average score | SD |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 78 | 10 |
| Rereading notes | 50 | 70 | 10 |
