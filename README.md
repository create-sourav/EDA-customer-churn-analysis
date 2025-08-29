📊 Telco Customer Churn — EDA Report
📌 Overview

This project analyzes the Telco Customer Churn dataset to understand patterns behind customer attrition.
The dataset contains 7,043 records and 21 features, covering demographics, account information, subscription services, billing details, and churn status (Yes/No).

The goal of this EDA is to explore what drives churn and generate insights that can guide customer retention strategies.

📂 Data Preparation

Loaded dataset WA_Fn-UseC_-Telco-Customer-Churn.csv.

Cleaned TotalCharges and MonthlyCharges (converted from string to numeric).

Converted SeniorCitizen column from binary (0/1) to categorical (Yes/No).

Verified dataset shape and data types.

🔍 Exploratory Analysis
1. Overall Churn Distribution

About 26.5% of customers churned while 73.5% stayed.

The dataset is imbalanced, with more non-churned customers.

2. Churn by Contract Type

Month-to-month contracts have the highest churn (~43%).

One-year contracts churn less (~11%).

Two-year contracts show very low churn (~3%).
➡️ Longer contracts strongly reduce churn.

3. Churn by Tenure

Churn is highest among new customers (0–6 months).

Churn steadily decreases as tenure increases.

Customers with >60 months tenure rarely churn.
➡️ Retention improves with customer age.

4. Churn by Senior Citizen & Gender

Senior Citizens churn more (42%) compared to non-seniors (24%).

Gender has little impact on churn; both male and female churn at similar rates.

5. Churn by Services

Customers without OnlineSecurity, TechSupport, or DeviceProtection are more likely to churn.

Fiber optic internet users churn more than DSL users.

Streaming services (TV/Movies) have weaker churn impact.

6. Churn by Payment Method

Churn distribution differs by PaymentMethod.

Customers using electronic check show higher churn compared to automatic payments (credit card, bank transfer).

✅ Key Insights

Contract length is the strongest churn driver.

Early-tenure customers are the most at risk.

Senior citizens churn at higher rates.

Lack of support/security services correlates with churn.

Payment method influences churn — auto-pay methods reduce risk.

💡 Recommendations (Future Work)

These steps go beyond EDA and can be considered for further project development:

🔹 Business Actions

Encourage month-to-month customers to switch to long-term contracts via promotions.

Improve onboarding experience for customers in the first 3–6 months.

Design senior-friendly support programs to improve retention.

Bundle add-ons like OnlineSecurity and TechSupport to reduce churn.

Promote auto-pay options to reduce churn linked to manual payments.

🔹 Analytical Extensions

Build a predictive model for churn (Logistic Regression or XGBoost).

Handle class imbalance (since only ~26% churn).

Use SHAP values to explain model predictions and identify top churn drivers.
