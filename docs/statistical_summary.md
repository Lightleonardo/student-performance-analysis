# Statistical Summary

## Distributions

Sample size: 6,607 students.

### Exam_Score

- Mean: 67.24
- Median: 67.00
- Standard deviation: 3.89
- Skewness: 1.64

Mean and median are close, but the mean sits slightly above the median and skewness is clearly positive (1.64), so the distribution has a right tail: a relatively small number of unusually high scores pulls the mean upward. Most scores cluster near 67, with a spread of about 3.9 points.

### Hours_Studied

- Mean: 19.98
- Median: 20.00
- Standard deviation: 5.99
- Skewness: 0.01

Mean and median are almost identical and skewness is near zero, so the distribution is roughly symmetric around 20 hours studied per week, with a spread of about 6 hours.

### Attendance

- Mean: 79.98
- Median: 80.00
- Standard deviation: 11.55
- Skewness: 0.01

Mean and median are almost identical and skewness is near zero, so attendance is also roughly symmetric around 80%, with a spread of about 11.5 percentage points.

## Sampling differences

The population mean Exam_Score is 67.24. Means of 20 samples of size n=30 ranged from 66.47 to 69.30, while means of 20 samples of size n=500 ranged only from 67.00 to 67.51. The smaller samples swing much more widely around the population mean than the larger ones, illustrating the Central Limit Theorem: larger samples produce more stable, reliable estimates of the population mean.

## Spreadsheet cross-check

The same statistics were recomputed in `spreadsheet/cross_check.xlsx` using `=AVERAGE`, `=MEDIAN`, `=STDEV.S`, and `=CORREL` formulas on the imported CSV data. The spreadsheet results matched the pandas results (Exam_Score mean 67.24, median 67, sample std 3.89; Hours_Studied vs. Exam_Score correlation 0.45). Pandas `.std()` defaults to sample standard deviation (ddof=1), so it matches Excel's `STDEV.S`; using population std (ddof=0 / `STDEV.P`) would not match.
