# 💳 Credit Card Customer Risk Analysis & Default Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![EDA](https://img.shields.io/badge/Project-EDA-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-purple)
![Seaborn](https://img.shields.io/badge/Visualization-Seaborn-lightblue)
![Matplotlib](https://img.shields.io/badge/Visualization-Matplotlib-red)
![Plotly](https://img.shields.io/badge/Visualization-Plotly-3F4F75?logo=plotly&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A comprehensive end-to-end data analytics project that analyzes credit card customer data to identify risk factors, segment customers by default probability, and deliver actionable business insights through interactive visualizations and a Power BI executive dashboard.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Analysis Phases](#analysis-phases)
- [Key Insights](#key-insights)
- [Strategic Recommendations](#strategic-recommendations)
- [Tools & Technologies](#tools--technologies)
- [How to Run](#how-to-run)



---

## 📖 Project Overview

Credit card issuers face significant challenges in identifying customers likely to default on their credit obligations. This project leverages **Exploratory Data Analysis (EDA)**, **feature engineering**, and **data visualization** to uncover the key behavioral and demographic factors that drive credit card default risk.

The project is delivered in two complementary formats:
- **Jupyter Notebook** — detailed EDA, statistical analysis, and business insights
- **Power BI Dashboard** — interactive executive-level risk monitoring dashboard
  
This project also lays the foundation for Machine Learning model development — the engineered features and risk segments created during EDA are directly usable for training classification models such as Logistic Regression, Random Forest, or XGBoost to predict customer default probability.

Future scope includes building and deploying an end-to-end ML pipeline with model explainability (SHAP values) to make AI-driven credit risk decisions transparent and business-ready.

---

## 🎯 Problem Statement

Credit card issuers face significant challenges in identifying customers who are likely to default on their credit obligations. Customer default can lead to financial losses, increased risk exposure, and reduced profitability for financial institutions. With a large and diverse customer base, it becomes difficult to manually analyze customer behavior and credit risk factors.

This project aims to analyze customer demographic, financial, and transactional data to identify patterns associated with credit card default risk. By leveraging exploratory data analysis (EDA) and predictive analytics, the study seeks to uncover key factors influencing default behavior and provide data-driven insights that can help financial institutions improve risk management and customer retention strategies.

---

## 📋 Objectives

**Primary Objective:**
To analyze credit card customer data and identify the factors that influence customer default risk, enabling better credit risk assessment and decision-making.

**Specific Objectives:**
- To understand the demographic profile of credit card customers based on age, gender, education level, and marital status.
- To analyze the relationship between customer income levels and credit default behavior.
- To examine how credit utilization indicators such as credit limit, transaction amount, and transaction frequency affect - default risk.
- To evaluate the impact of customer engagement metrics, including product count, bank contacts, and inactive months, on customer default status.
- To identify customer segments that exhibit higher probabilities of default.
- To perform exploratory data analysis (EDA) to uncover trends, patterns, and anomalies within the dataset.
- To determine the most influential variables contributing to credit card default.
- To create meaningful visualizations and dashboards that support business decision-making.
- To develop predictive insights that can assist financial institutions in identifying high-risk customers at an early stage.
- To provide recommendations for improving credit risk management and reducing potential financial losses.

---

## 📊 Dataset

**File:** `credit_card_customer_risk_csv.xlsx`

| Column | Description |
|--------|-------------|
| `customer_id` | Unique customer identifier |
| `default_flag` | Binary flag (1 = Default, 0 = No Default) |
| `default_status` | Categorical default label |
| `age` | Customer age |
| `gender` | Male / Female |
| `dependents` | Number of dependents |
| `education_level` | Highest education attained |
| `marital_status` | Married / Single / Unknown |
| `annual_income_range` | Income bracket (e.g., $40K–$60K) |
| `card_type` | Blue / Silver / Gold / Platinum |
| `months_on_book` | Tenure with institution (months) |
| `product_count` | Number of products held |
| `contacts_last_12m` | Bank contacts in past 12 months |
| `inactive_months_last_12m` | Months of inactivity in past 12 months |
| `credit_limit` | Assigned credit limit |
| `transaction_amount_last_12m` | Total transaction amount in past 12 months |
| `transaction_count_last_12m` | Total number of transactions in past 12 months |

---

## 📁 Project Structure

```
credit-card-risk-analysis/
│
├── Credit Card Customer Risk Notebook.ipynb            # Jupyter Notebook — EDA & Analysis
├── Credit Card Customer Risk Dashboard.pbix            # Power BI Executive Dashboard
├── credit_card_customer_risk.csv                       # Dataset
└── README.md                                           # Project documentation
```

---

## 🔍 Analysis Phases

### Phase 1 — Data Loading & Basic Understanding
- Loaded and inspected the dataset (shape, dtypes, statistical summary)
- Checked for missing values and duplicate records

### Phase 2 — Univariate Analysis
- Age distribution with mean/median reference lines
- Gender distribution analysis
- Annual income range distribution
- Credit limit distribution (skewness, mean vs. median)

### Phase 3 — Target Variable Analysis
- Default vs. non-default distribution
- Class balance assessment

### Phase 4 — Bivariate & Multivariate Analysis
- Default rates across demographics (age, gender, education, income)
- Credit utilization vs. default behavior
- Transaction activity patterns by risk group

### Phase 5 — Customer Engagement Analysis
- Impact of inactive months on default probability
- Relationship between bank contacts and default risk

### Phase 6 — Risk Segmentation
- Customer segmentation into Low / Medium / High Risk levels
- Risk level distribution visualization

### Phase 7 — Advanced Executive Visualizations
- **Sunburst Chart:** Hierarchical risk breakdown (Income → Card Type → Default Status)
- **Treemap:** Customer segmentation by income and education

### Phase 8 — Business Insights
Key findings derived from the analysis (see below).

### Phase 9 — Strategic Recommendations
Data-driven recommendations for risk management.

---

## 💡 Key Business Insights

1. **Portfolio is Financially Stable** — The majority of customers are non-defaulters, indicating a healthy credit portfolio with manageable risk exposure.

2. **Inactivity is a Strong Risk Indicator** — Customers with higher inactive months show a significantly greater likelihood of default, making inactivity an important early-warning signal.

3. **Age is Not a Primary Driver** — Similar age distributions across default and non-default groups suggest that behavioral and financial metrics matter more than demographics.

4. **Gender Has Limited Impact** — Default patterns are relatively consistent across male and female customers, indicating that gender has minimal influence on credit risk.

5. **Risk Segmentation Improves Allocation** — Most customers fall into the Low-Risk category, while a smaller segment contributes disproportionately to potential losses.

6. **Engagement Affects Performance** — Active customers demonstrate significantly better repayment behavior, while inactive customers are more likely to become high-risk accounts.

7. **Income Influences Credit Risk** — Customers with stronger financial profiles and higher income levels generally carry a lower probability of default.

8. **Credit Limits Should Be Assigned Strategically** — Customers with stable repayment behavior can be considered for higher credit limits, whereas high-risk customers should receive stricter credit exposure controls.

9. **Transaction Activity Reflects Customer Health** — Higher transaction frequency and spending levels are associated with more engaged and financially stable customers.

10. **Declining Transactions = Early Warning** — Falling transaction activity may signal an increased risk of future default, enabling proactive risk monitoring and intervention.


---

## 📌 Strategic Recommendations

1. Implement an **Early Warning System** based on inactivity and transaction trends
2. Regularly monitor **Medium and High-Risk** customer segments
3. Launch **retention campaigns** targeting inactive customers
4. Apply **risk-based credit limit management** policies
5. Develop a **machine learning model** for proactive default prediction
6. Create **customer engagement programs** to increase card usage and loyalty
7. Build **real-time executive dashboards** for continuous credit risk monitoring

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python 3.x | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib & Seaborn | Statistical visualizations |
| Plotly Express | Interactive charts (Sunburst, Treemap) |
| Jupyter Notebook | Analysis and reporting environment |
| Power BI | Executive dashboard and business reporting |
| Microsoft Excel | Dataset storage (.xlsx) |

---

## ▶️ How to Run

### Jupyter Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-risk-analysis.git
   cd credit-card-risk-analysis
   ```

2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly openpyxl
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Credit Card Customer Risk Notebook.ipynb
   ```

4. Update the dataset path in **Step 2** to point to the local file:
   ```python
   df = pd.read_csv("credit_card_customer_risk.csv")
   # or
   df = pd.read_excel("credit_card_customer_risk.csv")
   ```

### Power BI Dashboard

1. Open **Power BI Desktop**
2. Load `Credit Card Customer Risk Dashboard.pbix`
3. If prompted, update the data source path to your local dataset location

---

## 📄 License

Copyright © 2026 Uday Sahu

All Rights Reserved.

This project and all associated files, including but not limited to source code, notebooks, reports, dashboards, visualizations, documentation, and datasets, are the exclusive intellectual property of Uday Sahu.

No part of this project may be copied, reproduced, modified, distributed, published, sublicensed, displayed, transmitted, or sold in any form or by any means without the prior written permission of the copyright holder.

Permission is granted only to view this project for personal, educational, or portfolio evaluation purposes. Commercial use, redistribution, and creation of derivative works are strictly prohibited.

Unauthorized use, reproduction, or distribution of this project may result in legal action under applicable copyright laws.

For permissions or licensing inquiries, please contact the copyright holder directly.


---

## 🙋 Author

**Uday Sahu**
*Data Analytics Project | Credit Risk Domain*

