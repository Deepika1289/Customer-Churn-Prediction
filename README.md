# Customer Churn Prediction System

**Predicting subscription churn with explainable ML — 18% reduction in false negatives via SHAP-driven threshold optimization**

---

## Project Overview

An end-to-end machine learning pipeline that identifies customers at risk of churning before they leave. Built on a 50,000+ row customer dataset with full EDA, feature engineering, model comparison, and SHAP explainability — designed for direct use by business stakeholders.

| Detail | Information |
|---|---|
| **Dataset** | 50,000+ customer records with behavioral & demographic features |
| **Best Model** | XGBoost |
| **Best F1-Score** | Optimized via custom threshold tuning (+18% false-negative reduction) |
| **Explainability** | SHAP (SHapley Additive exPlanations) — top 3 churn drivers identified |
| **Task** | Binary classification — Churn / No Churn |

---

## Key Results

- **4 models compared**: Logistic Regression, Random Forest, SVM, XGBoost
- **18% reduction in false negatives** — customers at risk were less likely to go undetected after threshold optimization, directly protecting subscription revenue
- **Top 3 churn drivers identified** using SHAP values — actionable insights delivered to retention team
- **Cohort analysis dashboard** built in Seaborn for retention team review

---

## Tech Stack

`Python` `XGBoost` `Scikit-Learn` `SHAP` `SQL` `Pandas` `Seaborn` `Matplotlib` `Jupyter`

---

## Project Structure

```
Customer-Churn-Prediction/
├── data/
│   └── customer_data.csv          # Raw dataset (50K+ rows)
├── notebooks/
│   ├── 01_EDA.ipynb               # Exploratory data analysis
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training.ipynb    # All 4 models + comparison
│   └── 04_shap_analysis.ipynb     # SHAP explainability
├── src/
│   ├── preprocess.py
│   ├── train.py
│   └── evaluate.py
├── dashboard/
│   └── cohort_analysis.py         # Seaborn retention dashboard
├── requirements.txt
└── README.md
```

---

## Approach

### 1. EDA & Feature Engineering
- Full exploratory analysis on 50,000+ customer records
- Handled class imbalance, missing values, and categorical encoding
- Feature engineering on usage patterns, tenure, and support interactions

### 2. Model Training & Comparison
Trained and benchmarked 4 classifiers:

| Model | Notes |
|---|---|
| Logistic Regression | Baseline |
| Random Forest | Strong feature importance |
| SVM | Tested on scaled features |
| XGBoost | Best overall — selected for deployment |

### 3. Threshold Optimization
Default classification threshold (0.5) maximizes accuracy but not business value. By tuning the decision threshold specifically to minimize false negatives (missed churners), false negatives were reduced by **18%** — meaning fewer at-risk customers slipped through undetected.

### 4. SHAP Explainability
Used SHAP values to answer *why* the model predicted churn for each customer. The top 3 churn drivers were surfaced and presented to stakeholders in plain language — making the model's output actionable, not just accurate.

### 5. Cohort Analysis Dashboard
Built an interactive Seaborn dashboard showing retention trends by customer cohort — allowing the retention team to prioritize outreach.

---

## Quick Start

```bash
git clone https://github.com/Deepika1289/Customer-Churn-Prediction.git
cd Customer-Churn-Prediction

python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

pip install -r requirements.txt

jupyter notebook notebooks/01_EDA.ipynb
```

---

## Dependencies

```
scikit-learn
xgboost
shap
pandas
numpy
matplotlib
seaborn
jupyter
sqlalchemy
```

---

## Author

**N.V. Mani Deepika** — Data Scientist / ML Engineer  
[Portfolio](https://deepika-nuti.vercel.app) · [LinkedIn](https://linkedin.com/in/deepika-nuti-252118274) · [GitHub](https://github.com/Deepika1289)
