# Credit-Portfolio-Risk-Analytics
# Credit Risk Portfolio Analysis & Dashboard

A credit risk analytics project combining Python-based data preparation and predictive modelling with Power BI portfolio analysis and interactive risk reporting.

---

## 📌 Project Overview

Credit risk management requires financial institutions to understand the likelihood of borrowers defaulting and the potential financial impact of those defaults.

This project develops an end-to-end credit risk analysis pipeline that:

- Cleans and prepares loan-level data
- Performs exploratory data analysis
- Engineers predictive features
- Predicts Probability of Default (PD)
- Calculates Expected Loss
- Performs portfolio-level risk analysis
- Builds an executive Power BI dashboard
- Uses DAX to calculate dynamic credit-risk KPIs

The final output is an interactive credit-risk dashboard designed to support portfolio monitoring and risk-based decision making.

---

## 🎯 Business Objectives

The project aims to answer key credit-risk questions:

- How large is the loan portfolio?
- What is the portfolio's average Probability of Default?
- How much exposure is associated with the portfolio?
- What is the expected credit loss?
- What proportion of loans are in default?
- Which loan grades carry the greatest risk?
- Where is expected loss concentrated?
- How much exposure is associated with high-PD loans?
- Which areas of the portfolio require closer monitoring?

---

## 🗂️ Project Workflow

The project follows a five-stage Python workflow followed by Power BI reporting:

### 1. Data Cleaning

The raw loan dataset was cleaned and prepared for analysis.

Key activities included:

- Data quality checks
- Missing-value treatment
- Data-type validation
- Removal or treatment of unsuitable records
- Preparation of the analytical dataset

Notebook:

`01_data_cleaning.ipynb`

---

### 2. Exploratory Data Analysis

The portfolio was explored to understand borrower, loan and risk characteristics.

Analysis included:

- Loan amount distributions
- Interest-rate analysis
- Loan-grade composition
- Default patterns
- Portfolio segmentation
- Relationships between borrower characteristics and default outcomes

Notebook:

`02_eda.ipynb`

---

### 3. Feature Engineering

Additional variables were created to improve the predictive modelling process and support portfolio risk analysis.

Examples include:

- Loan-related features
- Borrower-related features
- Risk-related variables
- Exposure measures
- Loss Given Default (LGD)
- Model-ready predictors

Notebook:

`03_feature_engineering.ipynb`

---

### 4. Default Prediction

A predictive modelling pipeline was developed to estimate the Probability of Default (PD) for individual loans.

The predicted PD was then added to the portfolio dataset for downstream credit-risk analysis.

Notebook:

`04_default_prediction.ipynb`

---

### 5. Portfolio Risk Analytics

The predicted PD was combined with exposure and LGD assumptions to estimate expected credit losses and analyse portfolio-level risk.

The project uses the standard Expected Loss framework:

**Expected Loss = PD × LGD × Exposure**

Where:

- **PD** = Probability of Default
- **LGD** = Loss Given Default
- **Exposure** = Exposure at risk

Notebook:

`05_portfolio_risk_analytics.ipynb`

---

# 📊 Power BI Dashboard

The final scored portfolio dataset was imported into Power BI to create an executive credit-risk dashboard.

The dashboard provides:

### Portfolio KPIs

- Total Loans
- Total Exposure
- Average PD
- Expected Loss

### Risk KPIs

- Default Loans
- Default Rate
- NPL Ratio
- High Risk Loans
- High Risk Exposure

### Portfolio Analysis

- Exposure by Loan Grade
- Expected Loss by Loan Grade
- Average PD by Loan Grade
- Highest-risk loans
- Interactive portfolio filtering

---

## Dashboard Preview

![Credit Risk Dashboard](screenshots/credit_risk_dashboard.png)

---

## 📈 Portfolio Results

The current portfolio analysis contains approximately:

| Metric | Result |
|---|---:|
| Total Loans | 31,522 |
| Total Exposure | £304.6M |
| Average PD | 21.76% |
| Expected Loss | £34.0M |
| Default Loans | 6,807 |
| Default Rate | 21.59% |

Additional risk measures, including NPL Ratio and High Risk Exposure, are available interactively within the Power BI dashboard.

---

# 🧮 Power BI & DAX

Several DAX measures were created to support dynamic portfolio analysis.

Core measures include:

```text
Total Loans
Total Exposure
Average PD
Expected Loss
Default Loans
Default Rate
NPL Ratio
High Risk Loans
High Risk Exposure
