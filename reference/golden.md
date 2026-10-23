# Golden reference: a worked example

This document is for human review and should be kept outside the inputs supplied during an attempt. It shows one defensible analysis of the fictional studies. It is not an automated grading rule or a requirement to use this particular statistical method.

The arithmetic below has been reviewed by inspection. No statistical software or benchmark trial was run to produce this document.

## Evidence

The question is whether the practice-question groups had higher final exam scores than the rereading groups in the supplied studies. The exam scale, assessment time, group assignments, and participation details come from the shared conditions in [studies.md](../studies.md).

| School | Source | Practice n | Practice mean | Practice SD | Rereading n | Rereading mean | Rereading SD |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Oak | Table O1 | 50 | 76 | 10 | 50 | 70 | 10 |
| Pine | Table P1 | 50 | 74 | 10 | 50 | 70 | 10 |
| Maple | Table M1 | 50 | 78 | 10 | 50 | 70 | 10 |

There are three independent groups of participants, each split into two study-method arms: 300 students in total. Nobody is counted twice. All three comparisons use the same outcome and units, so a difference in exam points is directly interpretable.

## One analysis approach

This worked example uses a common-effect inverse-variance analysis with an approximate normal 95% confidence interval. It assumes the studies estimate a common underlying effect and that the two arms within each study, and the studies themselves, can be treated as independent for these calculations. These are assumptions of this reference analysis, not additional instructions for the participant.

For each school, subtract the rereading average from the practice-question average. A positive difference means the practice-question group scored higher.

The sampling variance of each difference is:

`variance = practice_SD^2 / practice_n + rereading_SD^2 / rereading_n`

Here, every comparison has variance `10^2 / 50 + 10^2 / 50 = 4` and standard error `sqrt(4) = 2` points. Its inverse-variance weight is `1 / 4 = 0.25`.

| School | Difference in points | Sampling variance | Weight | Share of total weight |
| --- | ---: | ---: | ---: | ---: |
| Oak | 76 - 70 = 6 | 4 | 0.25 | 1/3 |
| Pine | 74 - 70 = 4 | 4 | 0.25 | 1/3 |
| Maple | 78 - 70 = 8 | 4 | 0.25 | 1/3 |

The comparisons receive equal weight because their estimated precision is equal. The combined difference is:

`(0.25 * 6 + 0.25 * 4 + 0.25 * 8) / (0.25 + 0.25 + 0.25) = 6 points`

The variance of the combined estimate is `1 / 0.75 = 4/3`. Its standard error is `sqrt(4/3)`, approximately `1.1547` points.

Using a normal multiplier of approximately `1.96`, the 95% confidence interval is:

`6 +/- 1.96 * sqrt(4/3)`, approximately **3.74 to 8.26 points**.

Rounded numbers are for presentation; the expressions above retain the calculation details. This approach follows the standard inverse-variance framework described in the [Cochrane Handbook, Chapter 10](https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10).

## Example interpretation

In the three fictional studies, students who practiced questions scored higher on average than students who reread notes. The differences were 6, 4, and 8 exam points. Combining the studies using this analysis gives an estimated difference of 6 points, with an approximate 95% confidence interval from 3.74 to 8.26 points.

The interval describes uncertainty under the stated analysis assumptions. It is not the range of individual student scores, and it does not establish an identical effect at every school. The studies are invented, so these results do not establish the effectiveness of either method in real schools.

## Using the reference

Review whether an attempt used the supplied numbers accurately, connected its analysis to the sources, combined the studies coherently, and described uncertainty and limitations. An incomplete attempt can still show useful work.

The human instructions leave the method open. Other defensible methods, including methods that allow effects to vary across schools, may produce different uncertainty estimates. Treat a clearly explained methodological difference separately from a transcription mistake, arithmetic error, or unsupported conclusion. There is no required numerical score or pass/fail decision.
