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

Metric
Value
Total customers
7,043
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
Churn rate by segment
By contract type
Contract Type
Churn Rate
Month-to-month
42.7%
One year
11.3%
Two year
2.8%
By internet service
Internet Service
Churn Rate
Fiber optic
41.9%
DSL
19.0%
No internet service
7.4%
By payment method
Payment Method
Churn Rate
Electronic check
45.3%
Mailed check
19.1%
Bank transfer (automatic)
16.7%
Credit card (automatic)
15.2%
Month-to-month customers churn about 15x more than two-year contract customers — this gap is the core signal the whole project is built around.
Column reference
Category
Columns
Demographics
gender, SeniorCitizen, Partner, Dependents
Account info
tenure (months), Contract_*, PaperlessBilling, PaymentMethod_*
Services
PhoneService, MultipleLines, InternetService_*, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies
Billing
MonthlyCharges, TotalCharges
Engineered features
total_services (0–7, count of subscribed services), charge_ratio (TotalCharges ÷ MonthlyCharges — a proxy for spend consistency over tenure)
Target
Churn (Yes/No), Churn_num (1/0)

