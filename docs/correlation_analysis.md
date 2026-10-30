# Correlation Analysis

## Correlation matrix (numeric factors)

| Factor pair | Correlation |
|---|---|
| Attendance vs. Exam_Score | 0.58 |
| Hours_Studied vs. Exam_Score | 0.45 |
| Previous_Scores vs. Exam_Score | 0.18 |
| Sleep_Hours vs. Exam_Score | -0.02 |

The strongest relationship with Exam_Score is Attendance (r = 0.58), followed by Hours_Studied (r = 0.45). Previous_Scores has a weak positive relationship (r = 0.18). Sleep_Hours is effectively uncorrelated with Exam_Score (r = -0.02). The predictor variables are themselves largely uncorrelated with each other (all |r| < 0.03), so there is little multicollinearity among them.

The weakest relationship overall is Sleep_Hours vs. Exam_Score (r = -0.02), essentially zero.

## Correlation does not imply causation

Attendance and Exam_Score show a correlation of 0.58 in this dataset. This does not mean attending more classes causes a higher score. A plausible alternative explanation: a third, unmeasured variable, such as a student's motivation or health, could independently drive both better attendance and better exam performance (sometimes called a confounding variable). Without a controlled experiment, where attendance is deliberately varied while everything else is held constant, this dataset alone cannot distinguish "attendance causes better scores" from "something else causes both."
