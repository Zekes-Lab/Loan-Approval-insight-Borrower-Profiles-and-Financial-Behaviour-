# 🏦 Loan Approval insight: Borrower Profiles and Financial Behaviour

![Image](https://github.com/user-attachments/assets/9c05acf3-305d-41f8-a3df-68d15d7dc907

This project provides a detailed **Analysis and visualization** built using **Excel** and **Power BI**
The analysis focused on loan distribution,customer segmentation by( age, gender, education, employement status), repayment behavior, and credit risk patterns using a real-world loan dataset.

---

## 📊 Project Overview

The Analysis and visualization helps visualize and interpret key loan performance metrics:
- Total loan disbursed  
- Loan collector total  
- Average interest rate
- Overall repayment rate 

It also highlights:
- Customer segmentation by **age** and **gender**
- Loan disbursement by **purpose**
- Credit score relationships
- Public record averages
- Delinquency trends
- Loan amount distribution per income level

---

## 🧮 Dataset

- **Source:** [Kaggle – Loan Prediction Dataset 2025](https://www.kaggle.com/datasets/nabihazahid/loan-prediction-dataset-2025)
- **Observations:** 20,000  
- **Key Variables:**
  - `loan_amount`
  - `loan_purpose`
  - `credit_score`
  - `annual_income`
  - `debt_to_income_ratio`
  - `public_records`
  - `repayment_status`
  - `gender`, `age`, and `employment_status`

---

## ⚙️ Tools Used

| Tool | Purpose |
|------|----------|
| **Excel** | Data cleaning, pivot tables, regression analysis, and dashboard visualization |
| **Power BI** | Interactive dashboard creation and KPI visuals |

---
## 💻 Analysis Workflow

- Downloaded dataset and reviewed column definitions.  
- Cleaned and structured data. Created **Age Group**, **Credit Tier**, **Income Band** using Excel formulas.  
- Built pivot tables for each business question.  
- Designed charts and heatmaps using conditional formatting to highlight **risk** and **volume clusters**.  
- Performed multiple regression (*Interest Rate ~ Income + Credit Score + DTI*) using Excel’s **Data Analysis Toolpak**.  
- Validated model output: **R² = 0.32**, credit score holds predictive power, income and DTI do not.
---

## 📈 Regression Analysis Summary

The multiple regression analysis was used to evaluate how `credit_score`, `monthly_income`, and `debt_to_income_ratio` influence the **interest rate**.

| Metric | Value |
|---------|-------|
| Multiple R | 0.5689 |
| R Square | 0.3236 |
| Adjusted R Square | 0.3235 |
| Standard Error | 2.0091 |
| Observations | 20,000 |

**ANOVA Table**

| Source | df | SS | MS | F | Significance F |
|---------|----|----|----|---|----------------|
| Regression | 3 | 38618.17 | 12872.72 | 3189.06 | 0.000 |
| Residual | 19996 | 80714.35 | 4.04 |  |  |
| Total | 19999 | 119332.52 |  |  |  |

**Coefficients**

| Variable | Coefficient | Std. Error | t-Stat | P-Value | Lower 95% | Upper 95% |
|-----------|-------------|-------------|---------|----------|------------|------------|
| Intercept | 25.946 | 0.143 | 180.87 | 0.000 | 25.665 | 26.227 |
| Monthly_Income | 0.000001 | 0.000006 | 0.171 | 0.864 | -0.000011 | 0.000013 |
| Credit_Score | -0.01995 | 0.000204 | -97.78 | 0.000 | -0.02035 | -0.01955 |
| Debt_to_Income_Ratio | 0.02574 | 0.135 | 0.190 | 0.849 | -0.239 | 0.291 |

📊 **Interpretation:**
- **Credit score** has a strong and statistically significant *negative* effect on interest rate.
- **Monthly income** and **debt-to-income ratio** are not significant predictors.
- Model explains **32.4%** of the variance in interest rate (R² = 0.3236).

---

## 📉 Dashboard Visualizations

### Excel Dashboard
![WhatsApp Image 2025-10-17 at 23 06 42_71669dac](https://github.com/user-attachments/assets/a805a242-5509-4c82-a4ee-517bba6f4fb3)

*Figure 1. Loan Portfolio Dashboard (Excel)*  

### Power BI Dashboard
<img width="1262" height="729" alt="image" src="https://github.com/user-attachments/assets/93dee289-70d7-4e86-95fb-6a116619bd39" />
  
*Figure 2. Loan Portfolio Dashboard (Power BI)*  

Both dashboards include:
- KPI cards for major loan metrics  
- Pie, bar, and line charts for segmentation and performance  
- Gauge charts for credit and delinquency rates  

---

## 🔍 Key Insights

- **Credit score** is the strongest predictor of lower interest rates.
- **Old and matured applicants** received the highest loan amounts.
- **Employment type** and **loan purpose** significantly influence loan disbursement patterns.
- **Repayment rate (80%)** reflects relatively strong portfolio performance.
- Visual trends suggest the need to monitor **low-income** and **low-credit-score** segments closely.

---



  ## Author: Ogunyemi Ezekiel
Dashboard Title: Loan Portfolio Performance and Risk Insight Dashboard
