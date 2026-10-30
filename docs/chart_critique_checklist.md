# Chart Critique Checklist

For each chart, confirm:

- [x] Has a clear, specific title (not just the column name)
- [x] Both axes are labeled, with units if applicable
- [x] The chart type fits the data (histogram for distribution, scatter for relationship, heatmap for a matrix of values)
- [x] The y-axis starts at zero, or the truncation is clearly justified (a truncated axis can exaggerate differences)
- [x] Colors are distinguishable without relying on red/green alone
- [x] A one-sentence caption states the key takeaway, so the chart doesn't require the reader to infer it alone

## Applied to this project's charts

### 01_exam_score_distribution.png

- Title: "Distribution of Exam Scores" — specific, not just the column name.
- Axes: x = "Exam Score", y = "Number of Students"; both labeled.
- Type: histogram with KDE, appropriate for a distribution.
- Y-axis: starts at 0 (default), so differences are not exaggerated.
- Colors: single-color bars with KDE line, distinguishable without color reliance.
- Caption: Exam scores cluster around 67 with a slight right tail, indicating a few unusually high scores.

### 02_attendance_distribution.png

- Title: "Distribution of Attendance" — specific.
- Axes: x = "Attendance (%)", y = "Number of Students"; units included.
- Type: histogram with KDE, appropriate for a distribution.
- Y-axis: starts at 0.
- Colors: single-color bars with KDE line, distinguishable without color reliance.
- Caption: Attendance is roughly symmetric around 80%, with most students between roughly 65% and 95%.

### 03_study_hours_vs_score.png

- Title: "Study Hours vs Exam Score" — specific.
- Axes: x = "Hours Studied per Week", y = "Exam Score"; units included.
- Type: scatter plot with regression/trend line, appropriate for a relationship.
- Y-axis: not zero-based, but truncation is justified because exam scores only range from about 55 to 101; a zero baseline would waste space and obscure the relationship.
- Colors: scatter points and trend line are distinguishable without relying on red/green.
- Caption: More study hours are associated with higher exam scores, though with substantial scatter.

### 04_correlation_heatmap.png

- Title: "Correlation Between Numeric Factors" — specific.
- Axes: both axes list the compared factors; cells annotated with correlation values.
- Type: heatmap, appropriate for a matrix of values.
- Color scale: fixed from -1 to 1 with the "coolwarm" palette, so colors are distinguishable without relying on red/green alone.
- Caption: Attendance and study hours show the strongest positive correlations with exam score, while sleep hours are essentially uncorrelated.
