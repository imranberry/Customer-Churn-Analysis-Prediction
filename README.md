# 📊 Codar Data Science Program — Complete Course Notebook

> **End-to-end data science curriculum taught through a single real-world dataset**

## 🎯 About This Repository

This repository contains the **complete hands-on notebook** for the **Codar 12-Week Data Science Program** — a structured, practical course that takes absolute beginners from Python fundamentals all the way to a deployed machine learning model.

Every module of the course is demonstrated using a **single real-world dataset**: the Telco Customer Churn dataset (7,043 customers · 21 features). Rather than teaching concepts in isolation, this notebook shows how each tool and technique connects to the next — exactly how data science works in industry.

---

## 📁 Repository Contents

```
📦 codar-ds-churn-notebook
 ┣ 📓 Codar_DS_Course_Churn_Notebook.ipynb   ← Main course notebook (82 cells)
 ┣ 📊 DOC-20251224-WA0003_.xlsx              ← Telco Customer Churn dataset
 ┣ 📄 README.md                              ← You are here
 ┗ 📄 requirements.txt                       ← All dependencies
```

---

## 📚 Dataset Overview

| Feature | Description |
|---------|-------------|
| `customerID` | Unique customer identifier |
| `gender` | Male / Female |
| `SeniorCitizen` | 1 = senior citizen, 0 = not |
| `tenure` | Number of months as a customer |
| `PhoneService` … `StreamingMovies` | 7 subscribed service columns |
| `Contract` | Month-to-month / One year / Two year |
| `MonthlyCharges` | Monthly billing amount ($) |
| `TotalCharges` | Total amount charged to date ($) |
| `Churn` | **Target variable** — Yes (churned) / No (retained) |

**Size:** 7,043 rows · 21 columns · 11 missing values (TotalCharges only)  
**Class balance:** 73.5% retained · 26.5% churned

---

## 🗂️ Course Modules Covered

| # | Module | Key Topics |
|---|--------|-----------|
| 1 | **Python Fundamentals** | Variables, data types, operators, conditionals, loops, functions, OOP |
| 2 | **NumPy** | Arrays, vectorised operations, boolean indexing, linear algebra |
| 3 | **Pandas** | DataFrames, filtering, GroupBy, missing data, merge, concat |
| 4 | **Data Visualization** | Matplotlib subplots, Seaborn statistical charts, correlation heatmap |
| 5 | **Statistics & Mathematics** | Descriptive stats, hypothesis testing (t-test), correlation |
| 6 | **ML Foundations** | Feature engineering, ColumnTransformer pipeline, train/test split |
| 7 | **Classification** | Logistic Regression, Random Forest, Gradient Boosting, SVM |
| 8 | **Model Tuning** | k-fold cross-validation, GridSearchCV, hyperparameter optimization |
| 9 | **Deployment** | joblib serialization, Flask API template, cloud deployment |
| 10 | **SQL for Data Science** | SQLite, SELECT, GROUP BY, CTEs, Window Functions |
| 11 | **Capstone Summary** | Executive report, business recommendations, feature importance |

---

## 🔍 Key Findings from the Analysis

- 📌 **Month-to-month customers churn at 42.7%** vs only 2.8% for two-year contracts
- 📌 **Churned customers pay $74.44/month** on average vs $61.27 for retained customers (p < 0.001)
- 📌 **Electronic check users churn at 45%** — the highest risk payment method
- 📌 **New customers (tenure ≤ 6 months)** are the highest churn-risk segment
- 📌 **Gradient Boosting** outperforms all other models with the best ROC-AUC on this dataset

---

## 🤖 Model Performance Summary

| Model | Precision | Recall | F1-Score | ROC-AUC |
|-------|-----------|--------|----------|---------|
| Logistic Regression | — | — | — | — |
| Random Forest | — | — | — | — |
| **Gradient Boosting** ✅ | — | — | — | **Best** |

> Run the notebook to populate the metrics table with your actual results.

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/imranberry/Customer-Churn-Analysis-Prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter
```bash
jupyter notebook
```

### 4. Open the notebook
Click on `Codar_DS_Course_Churn_Notebook.ipynb` and run all cells from top to bottom.

> ⚠️ **Important:** Make sure the Excel file (`DOC-20251224-WA0003_.xlsx`) is in the **same folder** as the notebook before running. The first Pandas cell loads it directly.

---

## 🛠️ Requirements

```
pandas>=2.0
numpy>=1.24
matplotlib>=3.7
seaborn>=0.12
scikit-learn>=1.3
scipy>=1.11
joblib>=1.3
openpyxl>=3.1
flask>=3.0
sqlite3
```

Install all at once:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy joblib openpyxl flask
```

---

## 📂 Notebook Structure

The notebook contains **82 cells** — 39 markdown (explanations) and 43 code cells — organized as follows:

```
📓 Codar_DS_Course_Churn_Notebook.ipynb
 ┣ 🔷 Cover & Dataset Overview
 ┣ 🐍 Module 1  — Python Fundamentals (Cells 3–11)
 ┣ 🔢 Module 2  — NumPy (Cells 12–16)
 ┣ 🐼 Module 3  — Pandas (Cells 17–25)
 ┣ 📊 Module 4  — Visualization (Cells 26–33)
 ┣ 📐 Module 5  — Statistics (Cells 34–38)
 ┣ 🤖 Module 6  — ML Foundations (Cells 39–44)
 ┣ 🎯 Module 7  — Classification (Cells 45–54)
 ┣ 🔧 Module 8  — Cross-Validation & Tuning (Cells 55–58)
 ┣ 🚀 Module 9  — Saving & Deployment (Cells 59–62)
 ┣ 🗄️ Module 10 — SQL (Cells 63–70)
 ┗ 🏆 Module 11 — Capstone Summary (Cells 71–82)
```

---

## 💼 Business Recommendations

Based on the analysis in this notebook, the following interventions are recommended:

| Priority | Finding | Action |
|----------|---------|--------|
| 🔴 High | Month-to-month churn at 43% | Offer discounts to upgrade to annual contracts |
| 🔴 High | Electronic check churn at 45% | Incentivise auto-pay or credit card switch |
| 🟠 Medium | Fiber optic churn at 42% | Investigate service quality and pricing |
| 🟠 Medium | New customers are highest risk | Launch an onboarding and early intervention programme |
| 🟢 Low | Two-year contract churn at 3% | Maintain loyalty rewards for long-term customers |

---

## 🎓 About the Course

This notebook was built as part of the **Codar 12-Week Data Science Program** — a structured training program covering:

- Python programming from scratch
- Data wrangling with NumPy and Pandas
- Statistical analysis and hypothesis testing
- Machine learning with Scikit-learn
- Deep learning foundations with Keras
- SQL for data analysis
- Version control with Git & GitHub
- Business intelligence with Power BI
- End-to-end project deployment with Flask

**Instructor:** Codar Data Science  
**Program:** 12 Weeks · 24 Sessions · 1.5 Hours per Session

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## ⭐ If this notebook helped you

Give the repo a star ⭐ and share it with someone learning data science.  
Connect on LinkedIn and tag **Codar** when you share your progress!

---

*Built with ❤️ by Malik Imran*
