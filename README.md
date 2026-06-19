Credit-Wise Loan System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge"/>
</p>

> **An intelligent loan approval system powered by Machine Learning** — predicts whether a loan application should be approved or rejected based on applicant financial data.

---

## 📌 Project Overview

Banks and financial institutions receive thousands of loan applications daily. Manual review is slow, inconsistent, and prone to human bias. **Credit-Wise** automates this decision-making process using a trained ML classification model that evaluates applicant profiles and predicts loan eligibility with high accuracy.

This project covers the complete ML pipeline — from raw data exploration to a trained, evaluated model ready for deployment.

---

## 🎯 Problem Statement

Given an applicant's financial and demographic details, predict:
- ✅ **Approved** — the applicant is likely to repay the loan
- ❌ **Rejected** — the applicant poses a high credit risk

---

## 🔍 Dataset Features

| Feature | Description |
|---|---|
| `ApplicantIncome` | Monthly income of the applicant |
| `CoapplicantIncome` | Monthly income of the co-applicant |
| `LoanAmount` | Requested loan amount (in thousands) |
| `Loan_Amount_Term` | Repayment term in months |
| `Credit_History` | 1 = good credit history, 0 = poor |
| `Gender` | Male / Female |
| `Married` | Marital status |
| `Dependents` | Number of dependents |
| `Education` | Graduate / Not Graduate |
| `Self_Employed` | Employment type |
| `Property_Area` | Urban / Semiurban / Rural |
| `Loan_Status` | **Target** — Y (Approved) / N (Rejected) |

---

## 🛠️ Tech Stack

- **Python 3.x**
- **Pandas** — data loading and manipulation
- **NumPy** — numerical operations
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — ML modeling, preprocessing, evaluation
- **Jupyter Notebook** — interactive development environment

---

## 🔄 ML Pipeline

```
Raw Data → EDA → Data Cleaning → Feature Engineering → Model Training → Evaluation → Prediction
```

**Step-by-step breakdown:**

1. **Exploratory Data Analysis (EDA)** — visualize distributions, correlations, and class imbalance
2. **Data Cleaning** — handle missing values using median/mode imputation
3. **Feature Engineering** — log-transform skewed features (LoanAmount, Income), encode categoricals
4. **Train-Test Split** — 80% training, 20% testing
5. **Model Training** — Logistic Regression and Decision Tree Classifier
6. **Evaluation** — Accuracy, Confusion Matrix, Classification Report
7. **Prediction** — predict loan approval on new applicant data

---

## 📊 Key Findings from EDA

- Applicants with **good credit history** are ~8x more likely to get approved
- **Semiurban area** applicants have the highest approval rate
- Higher **combined income** (applicant + coapplicant) improves approval odds
- `LoanAmount` and `ApplicantIncome` are right-skewed — log transformation improves model performance

---

## 📈 Model Performance

| Model | Accuracy |
|---|---|
| Logistic Regression | ~80% |
| Decision Tree | ~78% |

> Credit History is by far the most important feature — accounting for the majority of predictive weight.

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/ayush10mishra-hash/credit-wise-loansystem.git
cd credit-wise-loansystem
```

**2. Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**3. Launch the notebook**
```bash
jupyter notebook credit_wise.ipynb
```

**4. Run all cells** — the notebook walks through EDA, preprocessing, training, and evaluation end to end.

---

## 📁 Project Structure

```
credit-wise-loansystem/
│
├── credit_wise.ipynb      # Main Jupyter notebook (EDA + Model)
└── README.md              # Project documentation
```

---

## 🔮 Future Improvements

- [ ] Add Random Forest and XGBoost models for comparison
- [ ] Build a web interface using Flask or Streamlit
- [ ] Deploy model as a REST API
- [ ] Add SHAP values for model explainability

---

## 👤 Author

**Ayush Mishra** — AI & ML Engineer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ayush-mishra-5b015635b)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/ayush10mishra-hash)

---

⭐ If you found this project useful, please consider giving it a star!

