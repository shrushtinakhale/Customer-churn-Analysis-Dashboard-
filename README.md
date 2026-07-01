📊Customer Churn Analysis & Dashboard
An end-to-end customer churn project for a telecom company — combining exploratory data analysis, statistical testing, predictive modeling (Python), and an interactive Power BI dashboard for business stakeholders.
📌 Project Overview
Customer churn is one of the biggest revenue risks for subscription-based telecom businesses. This project analyzes a telecom customer dataset to:
Understand why customers churn
Identify key drivers of churn using statistical analysis
Build predictive models to flag at-risk customers
Present findings through an interactive Power BI dashboard for non-technical stakeholders
🗂️ Repository Structure
├── telco_churn_cleaned.csv        # Cleaned dataset used for analysis, modeling, and the dashboard
├── customer_churn_dashboard.pbix  # Power BI dashboard (interactive report)
├── dashboard_preview.png          # Static preview image of the Power BI dashboard
├── 1_EDA_and_Data cleaning.ipynb       # Part 1: Data cleaning, EDA, feature engineering, and ML modeling
├── 2_Statistical_Analysis_and_modeling.ipynb   # Part 2: Hypothesis testing and statistical analysis of churn drivers
└── README.md

🧹 Dataset
File: telco_churn_cleaned.csv
Rows: 7,043 customers
Columns: 30 (post-cleaning / feature-engineered)
Missing values: 0 (post-cleaning)
This is the classic IBM Telco Customer Churn dataset — one row per customer at a telecom company, covering demographics, subscribed services, account/billing details, and whether they churned.
Headline numbers (from the cleaned data)

Metric              | Value
Total customers.    | 7,043
Churned customers
1,869
Retained customers
5,174
Overall churn rate
26.5%
Average tenure
32.4 months
Average monthly charges
$64.76
Average total charges
$2,279.73
