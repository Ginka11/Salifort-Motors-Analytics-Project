# Salifort Motors Employee Churn Analysis

An HR analytics capstone project completed as part of the **Google Advanced Data Analytics Professional Certificate**. The project explores employee attrition drivers and develops a binary classification workflow to support retention decisions.

## Business Question

What factors are most strongly associated with employees leaving Salifort Motors, and how can HR identify higher-risk employee groups?

## Dataset

- 14,999 employee records
- 10 original variables
- Target: `left`
- Main features: satisfaction, evaluation score, project count, monthly hours, tenure, promotion history, department, salary and work accidents

## Workflow

1. Defined the HR problem and stakeholders using the PACE framework.
2. Cleaned column names and reviewed data quality.
3. Explored attrition patterns with Pandas, Matplotlib and Seaborn.
4. Prepared categorical variables and created a stratified train/test split.
5. Compared an interpretable Logistic Regression baseline with a tree-based approach.
6. Translated findings into retention recommendations and ethical-use guidance.

## Key Findings

- Low satisfaction was the strongest recurring indicator of attrition.
- Employees with very high project loads and long monthly hours showed clear burnout risk.
- The 3–5 year tenure range, especially around year 4, was a critical retention period.
- High evaluation scores did not protect against turnover when workload was excessive.

## Reported Model Results

The notebook reports approximately:

- Logistic Regression accuracy: **82%**
- Random Forest F1-score: **94–95%**
- Random Forest precision: **97%**
- Random Forest recall: **91%**

These figures are retained as project results from the completed notebook. A production implementation would require additional validation, leakage checks, fairness testing and monitoring.

## Recommendations

- Cap concurrent project assignments at five where operationally feasible.
- Flag sustained monthly workloads above roughly 220 hours for review.
- Introduce stay interviews and career-development discussions near the fourth year of tenure.
- Reward sustainable output rather than overtime alone.
- Use predictions to support employees, not to penalize or surveil them.

## Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Contents

```text
Salifort-Motors-Analytics-Project/
├── Salifort_Motors_Employee_Churn_Prediction.ipynb
├── requirements.txt
└── README.md
```

## Run Locally

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Open `Salifort_Motors_Employee_Churn_Prediction.ipynb` and run the cells in order. The course notebook originally loaded the dataset in its hosted environment, so a local run may require adding the source CSV and updating its path.
