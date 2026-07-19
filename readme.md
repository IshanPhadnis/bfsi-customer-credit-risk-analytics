# BFSI Customer Credit Risk Analytics

An end-to-end **Banking & Financial Services (BFSI)** analytics project that simulates the work of a **Data Analyst** in a retail bank's Credit Risk and Customer Analytics team. Using **SQL (BigQuery)** and **Tableau**, this project analyzes customer behavior, credit risk, transaction patterns, fraud indicators, and portfolio performance to generate actionable business insights and executive-level recommendations.

The project is inspired by real-world analytics performed at leading financial institutions such as **American Express, JPMorgan Chase, Citi, HSBC, HDFC Bank, and ICICI Bank**, focusing on how data supports lending decisions, customer segmentation, fraud monitoring, and business strategy.

---

# 🎯 Business Objective

The objective of this project is to answer critical business questions such as:

- Which customers are most likely to default?
- Which customer segments generate the highest lifetime value?
- Are customers utilizing too much of their available credit?
- Which customers should be targeted for premium card upgrades?
- What spending patterns indicate potential fraud?
- Which customer segments should receive retention or cross-selling campaigns?

---

# 📂 Dataset

**Credit Card User Behavior & Default Dataset**

The dataset contains **10,000 customer records**, with each row representing a unique customer. It is a single-snapshot dataset — there is no time-series, transaction-level, or credit-limit/exposure data — so all analysis is framed around what this snapshot can actually support.

### Customer Information
- Customer ID
- Age
- Gender
- Marital Status
- Education Level
- Employment Status

### Financial Information
- Annual Income
- Credit Score
- Number of Credit Lines
- Debt-to-Income Ratio
- Credit Utilization Ratio

### Customer Behaviour
- Total Spend
- Number of Transactions
- Merchant Diversity
- City Diversity
- Customer Lifetime Value (CLV)

### Risk Indicators
- Late Payments
- Default Status
- Fraud Transaction Count

---

# 🛠️ Tech Stack

| Tool | Purpose |
|-------|----------|
| **Google BigQuery** | SQL analysis and business intelligence |
| **Tableau** | Interactive dashboards and executive reporting |
| **GitHub** | Project documentation and portfolio |
| **Python (Phase 2)** | Exploratory Data Analysis (EDA), data cleaning, feature engineering, and predictive analytics |

---

# 📁 Project Structure

```text
BFSI_Customer_Credit_Risk_Analytics/

│
├── 01_Customer_Intelligence.md
├── 02_Credit_Risk_Analytics.md
├── 03_Fraud_Analytics.md
├── 04_Customer_Behaviour_Analytics.md
├── 05_Portfolio_Analytics.md
├── 06_Strategic_Analytics.md
├── 07_Executive_Summary_BI.md
│
├── SQL/
├── Tableau/
├── README.md
```

---

# 📊 Business Analytics Modules

## Customer Intelligence
- Percentile-based customer segmentation (Low/Medium/High/VIP)
- CLV benchmarking by income and demographic group
- Weighted customer scoring (CLV, credit score, utilization, default history)
- High-revenue / high-risk customer identification

## Credit Risk Analytics
- Default driver analysis
- Composite Risk Scoring (credit score, utilization, DTI, late payments)
- Default probability by utilization and income bands
- Overleveraged customer identification
- Rule-based Early Warning flagging

## Fraud Analytics
- Fraud profile identification
- Fraud incidence by CLV tier and transaction frequency
- Merchant diversity vs. fraud correlation
- Fraud-adjusted profitability
- Manual review candidate flagging

## Customer Behaviour Analytics
- Pareto analysis (spend concentration)
- Spend-vs-demographic-average comparison
- Multi-dimensional segmentation (spend, frequency, utilization)
- Engagement ranking

## Portfolio Analytics
- Portfolio concentration analysis
- Risk-driving segment identification
- Risk-adjusted CLV by segment
- Spend/income-based exposure proxies
- Z-score outlier detection
- Profitability vs. risk matrix

## Strategic Analytics
- Premium upgrade candidate identification
- Credit line increase/decrease recommendations
- Cross-sell and retention targeting
- Executive Credit Risk Dashboard
- Executive Portfolio Review

---

# 🔍 Methodology

This project follows a **question-driven analytics approach**, where every analysis begins with a real business question rather than a predefined SQL query.

Each analysis includes:

1. Business Question
2. SQL Solution
3. Key Metrics
4. Business Insights
5. Strategic Recommendations
6. Business Impact

This workflow mirrors how analysts operate in financial institutions by translating business problems into data-driven decisions.

---

# 📈 Dashboard

Interactive Tableau dashboards present:

- Executive KPIs
- Customer Segmentation
- Credit Risk Overview
- Transaction Analytics
- Fraud Monitoring
- Business Performance Summary

---

# 💼 Key Skills Demonstrated

- Advanced SQL (CTEs, Window Functions, Subqueries, CASE Statements)
- Business Intelligence
- Credit Risk Analytics
- Customer Segmentation
- Customer Lifetime Value (CLV)
- Fraud Analysis
- Banking KPI Reporting
- Data Visualization (Tableau)
- Executive Storytelling
- Business Recommendations

---

# 🚀 Future Enhancements

### Phase 2 – Python

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Statistical Analysis

### Phase 3 – Machine Learning

- Loan Default Prediction
- Customer Risk Scoring
- Probability of Default (PD) Modeling
- Customer Risk Classification

---

# 🎯 Project Goal

The goal of this project is to demonstrate the end-to-end analytical workflow expected of a **Data Analyst** or **Business Analyst** in the Banking & Financial Services industry—from writing complex SQL and building executive dashboards to generating actionable business recommendations that support credit risk management, customer growth, and strategic decision-making.
