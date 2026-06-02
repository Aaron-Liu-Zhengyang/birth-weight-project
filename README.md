# Infant Birth Weight Analysis & Modeling
> **Course**: Reproducible Research

---

## 1. Project Overview
This project provides a fully reproducible data science pipeline to analyze and predict infant birth weights using the `birthwt` dataset. The workflow is split into three sequential Jupyter Notebooks:
1. `01_data_cleaning.ipynb` – Data preprocessing, type conversion, and initial formatting.
2. `02_EDA.ipynb` – Exploratory data analysis, feature engineering, and statistical visualizations.
3. `03_modeling_stats.ipynb` – Multiple linear regression modeling, diagnostics, and replication of specific predictions.

---

## 2. Directory Structure
```text
.
├── data/
│   ├── birthwt.csv
│   └── birthwt_final_cleaned.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_EDA.ipynb
│   └── 03_modeling_stats.ipynb
└── README.md
```

3. Environment & Dependencies
This project requires Python 3.x. To ensure exact reproducibility of the results and figures, install the required packages using pip:

Bash
pip install pandas numpy matplotlib seaborn statsmodels scipy

4. Execution Order
To reproduce the findings without errors, please open and execute the notebooks in the notebooks/ folder in the following strict order:

01_data_cleaning.ipynb

Input: data/birthwt.csv

Output: Generates the processed dataset data/birthwt_final_cleaned.csv.

02_EDA.ipynb

Input: data/birthwt_final_cleaned.csv

Action: Analyzes underlying distributions, derives custom risk features, and computes variable correlations.

03_modeling_stats.ipynb

Input: data/birthwt_final_cleaned.csv

Action: Fits the final regression model, evaluates residuals, and outputs the sample prediction interval.