# Golden reference: G01 specified analysis

This document is for human review and should be kept outside the inputs supplied during an attempt. It works through the analysis required by the participant-visible [G01 calculation card](../studies.md#g01-calculation-card). The card specifies the method and precision; this reference provides the expected calculations and an example explanation. It is not an automated grader.

The arithmetic below has been reviewed by inspection. No statistical software or benchmark trial was run to produce this document.

## Evidence

The question is whether the practice-question groups had higher final exam scores than the rereading groups in the supplied studies. The exam scale, assessment time, group assignments, and participation details come from the shared conditions in [studies.md](../studies.md).

| School | Source | Practice n | Practice mean | Practice SD | Rereading n | Rereading mean | Rereading SD |
| --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Oak | Table O1 | 50 | 76 | 10 | 50 | 70 | 10 |
| Pine | Table P1 | 50 | 74 | 10 | 50 | 70 | 10 |
| Maple | Table M1 | 50 | 78 | 10 | 50 | 70 | 10 |

There are three independent groups of participants, each split into two study-method arms: 300 students in total. Nobody is counted twice. All three comparisons use the same outcome and units, so a difference in exam points is directly interpretable.

## Specified analysis

Following the calculation card, use all three schools in a common-effect inverse-variance analysis with an approximate normal 95% confidence interval. Assume the studies estimate a common underlying effect and treat the two arms within each study, and the studies themselves, as independent. Use the supplied sample SDs and group sizes, without adding a between-school variance term.

For each school, subtract the rereading average from the practice-question average. A positive difference means the practice-question group scored higher.

The sampling variance of each difference is:

`variance = practice_SD^2 / practice_n + rereading_SD^2 / rereading_n`

Here, every comparison has variance `10^2 / 50 + 10^2 / 50 = 4` and standard error `sqrt(4) = 2` points. Its inverse-variance weight is `1 / 4 = 0.25`.

| School | Difference in points | Sampling variance | Weight | Share of total weight |
| --- | ---: | ---: | ---: | ---: |
| Oak | 76 - 70 = 6.00 | 4 | 0.25 | 1/3 |
| Pine | 74 - 70 = 4.00 | 4 | 0.25 | 1/3 |
| Maple | 78 - 70 = 8.00 | 4 | 0.25 | 1/3 |

The comparisons receive equal weight because their estimated precision is equal. The combined difference is:

`(0.25 * 6 + 0.25 * 4 + 0.25 * 8) / (0.25 + 0.25 + 0.25) = 6 points`

The variance of the combined estimate is `1 / 0.75 = 4/3`. Its standard error is `sqrt(4/3)`, approximately `1.1547` points.

Using exactly `1.96` as the card's normal multiplier, the approximate 95% confidence interval is:

`6 +/- 1.96 * sqrt(4/3)`, approximately **3.74 to 8.26 points**.

The required combined estimate is **6.00 points**, with an approximate **95% confidence interval of 3.74 to 8.26 points**. Keep full precision in the calculations and round only the reported differences and interval limits to two decimal places. The displayed standard error is illustrative; the interval uses `sqrt(4/3)` without intermediate rounding. This approach follows the standard inverse-variance framework described in the [Cochrane Handbook, Chapter 10](https://www.cochrane.org/authors/handbooks-and-manuals/handbook/current/chapter-10).

## Example interpretation

In the three fictional studies, students who practiced questions scored higher on average than students who reread notes. The differences were 6.00, 4.00, and 8.00 exam points. Combining the studies using the specified analysis gives an estimated difference of 6.00 points, with an approximate 95% confidence interval from 3.74 to 8.26 points.

The interval describes uncertainty under the stated analysis assumptions. It is not the range of individual student scores, and it does not establish an identical effect at every school. The studies are invented, so these results do not establish the effectiveness of either method in real schools.

## Using the reference

Review the extracted numbers and source references, then each school's difference, variance and weight, the combined estimate, the interval, and the explanation. Record completed stages, numerical errors, missing work, and departures from the calculation card separately. An incomplete attempt can still show useful work.

Compare reported differences and interval limits after rounding to two decimal places. Numerically equivalent forms such as `6`, `6.0`, and `6.00` represent the same result. Different tools, equivalent implementations of the formulas, and explanations in the participant's own words are acceptable. A different statistical method does not fulfill G01's specified analysis and should be recorded as a departure from the card, separately from any arithmetic errors. There is no required numerical score or pass/fail decision.

The equal group sizes and SDs make the weighted estimate equal to the plain average of the three differences. Review the supporting calculations as well as the final number; a result of 6.00 alone does not demonstrate that the participant used all three studies or followed the card.
