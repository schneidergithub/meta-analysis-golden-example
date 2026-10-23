# Meta-analysis golden example

A small, human-readable task about combining results from three fictional studies. It contains four documents and no runnable code.

| File | Purpose |
| --- | --- |
| [instruction.md](instruction.md) | The approved human instructions, preserved exactly. |
| [studies.md](studies.md) | Three short fictional school studies and the G01 calculation card. |
| [reference/golden.md](reference/golden.md) | The worked specified analysis and an example interpretation for human review. |

The studies compare practice questions with rereading notes. All data, schools, and study descriptions are invented for this example. They are not evidence about real teaching effectiveness.

G01 measures whether a participant can extract the evidence and reproduce the analysis specified in the calculation card in `studies.md`. The card supplies the method, formulas, and reporting precision; the golden reference works through the expected result. Different calculation tools and explanations are welcome, provided the calculations follow the card. The approved text in `instruction.md` is unchanged. There is no automated score or pass/fail gate. Partial work can still be reviewed.

For a future attempt, supply only `instruction.md` and `studies.md`. Keep this README and `reference/golden.md` outside the participant's or model's accessible inputs. The repository itself does not enforce that separation.

The reference arithmetic has been reviewed by inspection. No analysis program, test suite, grader, container, or benchmark trial was run during creation. Any future execution requires a separate instruction.
