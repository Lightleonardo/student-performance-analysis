# Student Performance Analysis

Statistical and visual analysis of student exam performance, exploring score
distributions, attendance patterns, sampling behavior, and the relationship
between study habits and results.

## Dataset

Student Performance Factors from Kaggle: https://www.kaggle.com/datasets/lainguyn123/student-performance-factors
(6,607 rows, 20 columns)

## Setup

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Running

```powershell
jupyter notebook
# open notebooks/analysis.ipynb, run all cells top to bottom
```

## Project structure

| Folder / File | Description |
|---|---|
| `data/raw/` | Raw dataset (`StudentPerformanceFactors.csv`) |
| `notebooks/analysis.ipynb` | Main analysis notebook |
| `charts/` | Generated charts (`01`-`04_*.png`) |
| `spreadsheet/cross_check.xlsx` | Independent spreadsheet cross-check |
| `docs/statistical_summary.md` | Distribution and sampling statistics |
| `docs/correlation_analysis.md` | Correlation analysis and causation caveat |
| `docs/chart_critique_checklist.md` | Chart critique checklist applied to project charts |
| `docs/insights.md` | Five written insights |
| `requirements.txt` | Python dependencies |
| `README.md` | Project overview |
| `.gitignore` | Git ignore rules |
