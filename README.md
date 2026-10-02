# Customer Churn Prediction

Predicting which telecom customers are likely to leave, using machine learning, so the company can act before they go.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MeghanaGS26/customer-churn-prediction/blob/main/Customer_Churn_Prediction.ipynb)

## Problem Statement
Losing customers is expensive. This project identifies customers at high risk of churning and finds the factors that drive them to leave.

## Dataset
Telco Customer Churn (IBM sample dataset): 7,043 customers with 20 features such as contract type, tenure, monthly charges, internet service and payment method. About 26% of customers churned.

## Approach
1. **Data cleaning:** fixed the `TotalCharges` column, dropped `customerID`, encoded the target as 0/1
2. **Exploratory data analysis:** churn rate by contract, internet service, payment method and tenure
3. **Preprocessing:** one-hot encoding, stratified 80/20 train-test split
4. **Models:** Logistic Regression, Random Forest, XGBoost (class imbalance handled with class weights)
5. **Evaluation:** accuracy, precision, recall, F1, ROC-AUC, confusion matrix

## Results
| Model | Accuracy | Recall | ROC-AUC |
|---|---|---|---|
| Logistic Regression | ... | 0.786 | 0.84 |
| Random Forest | ... | ... | ... |
| XGBoost | ... | ... | ... |

**Best model:** Logistic Regression, which catches about 79% of customers who actually churn.

## Key Insights
- Month-to-month contract customers churn far more than those on 1- or 2-year contracts.
- Customers in their first year are the most likely to leave.
- Fiber optic and electronic check customers show higher churn.
- Customers without tech support or online security churn more.

## Business Recommendations
1. Offer incentives to move month-to-month customers to annual plans.
2. Run onboarding and check-in programs for customers in their first 12 months.
3. Bundle tech support and online security into plans.
4. Target customers flagged as high risk with retention offers.

## Tools Used
Python, pandas, NumPy, scikit-learn, XGBoost, matplotlib, seaborn, Google Colab

## How to Run
Click the "Open in Colab" badge above and choose **Runtime → Run all**.
