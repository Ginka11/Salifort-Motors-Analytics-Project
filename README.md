# Salifort Motors Employee Attrition EDA

An exploratory HR analytics capstone completed through the **Google Advanced Data Analytics Professional Certificate**. The notebook examines employee attrition patterns and translates the observed data into questions and recommendations for HR.

> This repository intentionally presents the work as **exploratory data analysis**, not as a validated prediction model. The committed notebook does not contain estimator fitting or model evaluation code, so earlier model-performance claims are not published here.

## Business Question

Which employee characteristics and workload patterns are associated with attrition in the supplied Salifort Motors dataset?

## Dataset

The persisted notebook outputs verify:

- **14,999** original rows and **10** variables
- **3,008** exact duplicate rows identified
- **11,991** records after duplicate removal
- **10,000** employees who stayed
- **1,991** employees who left
- **16.60%** attrition rate after duplicate removal

The course notebook uses `HR_capstone_dataset.csv`. The repository does not redistribute that CSV. The underlying public dataset is available from [HR Analytics and Job Prediction on Kaggle](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction); review its dataset page for attribution and usage terms.

## Analysis Completed

- Standardized and reviewed the source columns.
- Checked data types, missing values, duplicates, and tenure outliers.
- Removed exact duplicate rows for the analytical dataframe.
- Compared attrition across:
  - satisfaction level
  - project count
  - monthly working hours
  - salary band
  - evaluation score
  - tenure
  - department
- Documented responsible-use considerations for employee analytics.

## HR Questions Raised by the EDA

The visual analysis suggests areas for HR to investigate further rather than causal conclusions:

- Whether extreme workloads coincide with lower retention.
- Whether project allocation is balanced across teams.
- Whether the 3â€“5 year tenure period needs targeted career conversations.
- Whether promotion, salary, and workload policies interact with satisfaction.

## Recommendations

- Monitor sustained workload and project allocation at team level.
- Use stay interviews to understand employee experience before attrition occurs.
- Review promotion and career-path opportunities alongside satisfaction signals.
- Treat analytical findings as prompts for support, not as grounds for punitive employee decisions.
- Validate any future predictive model for leakage, fairness, calibration, and drift before use.

## Repository Contents

```text
salifort-employee-attrition-eda/
â”œâ”€â”€ Salifort_Motors_Employee_Attrition_EDA.ipynb
â”œâ”€â”€ requirements.txt
â””â”€â”€ README.md
```

## Run Locally

```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook
```

Download the dataset, save it as `HR_capstone_dataset.csv` beside the notebook, then run `Salifort_Motors_Employee_Attrition_EDA.ipynb` in order.

## Reproducibility Status

The exploratory sections contain persisted outputs, but the notebook was originally completed in a hosted course environment. A future modeling iteration should start from a clean kernel, add an explicit preprocessing pipeline, fit and evaluate candidate models, and publish only metrics produced by committed code.

## Technologies

Python | Pandas | NumPy | Matplotlib | Seaborn | Jupyter Notebook

