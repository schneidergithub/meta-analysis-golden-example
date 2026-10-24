# Supplied studies

These are fictional studies created for this exercise. Each school represents one study.

## Shared study conditions

Each of the three schools compared two groups of students.

- One group of students used practice questions to prepare for an exam.
- The other group prepared for the exam by rereading their notes instead.

Both groups started with the same course materials. Students studied for the same amount of time over six weeks, then took the same exam.

Within each school, 100 students were randomly assigned, 50 to practice questions and 50 to rereading notes.

Exam scores range from 0 to 100 points. The tables report each group's [average score](glossary.md#average-score) and [sample standard deviation](glossary.md#standard-deviation), both in points.

## Calculation Method

See the [shared glossary](glossary.md) for explanations of the terms used below.

### 1. Calculate each school's result

**[School's estimated difference](glossary.md#schools-estimated-difference)**

> **School's estimated difference =**<br>
> **Practice-question group**'s average score<br>
> − **Rereading group**'s average score

A positive difference means the practice-question group scored higher on average.

**[Variance of the estimated difference](glossary.md#variance-of-the-estimated-difference)**

For each of the two groups (the **practice-question group** and **rereading group**) calculate:

(Standard Deviation × Standard Deviation) ÷ number of students

Add the two amounts you just calculated to get the variance of the school's estimated difference.

**[Weight](glossary.md#weight)**

Weight = 1 ÷ variance of the estimated difference

### 2. Combine the schools

Add the three weights to get the **[total weight](glossary.md#total-weight)**.

Multiply each school's estimated difference by its weight to get its **[weighted difference](glossary.md#weighted-difference)**. Add the three weighted differences, then divide by the total weight:

**[Combined difference](glossary.md#combined-difference) = sum of the weighted differences ÷ total weight**

### 3. Calculate the uncertainty

**[Standard error](glossary.md#standard-error) = square root of (1 ÷ total weight)**

This measures the uncertainty in the combined difference.

**[Margin](glossary.md#margin) = 1.96 × standard error**

Calculate the interval limits.

**Lower limit = combined difference − margin**

**Upper limit = combined difference + margin**

The limits form the approximate [95% confidence interval](glossary.md#95-confidence-interval).

For this calculation, assume the actual difference between the two exam preparation methods is the same at all three schools, even though their reported results differ. Treat results from different groups and schools as [independent](glossary.md#independent-results).

### Show your work

List the numbers you used and name the table each came from. For each school, show its estimated difference, variance of the estimated difference, and weight. Then show the weighted differences, combined difference, and confidence interval. Explain the finding and uncertainty in your own words.

## Oak School

**Table O1. Oak School exam results after six weeks**

| Exam preparation method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 76 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Pine School

**Table P1. Pine School exam results after six weeks**

| Exam preparation method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 74 | 10 |
| Rereading notes | 50 | 70 | 10 |

## Maple School

**Table M1. Maple School exam results after six weeks**

| Exam preparation method | Students | Average score | Standard Deviation |
| --- | ---: | ---: | ---: |
| Practice questions | 50 | 78 | 10 |
| Rereading notes | 50 | 70 | 10 |
