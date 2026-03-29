# Netflix Churn Prediction — Logistic Regression

Machine learning project that predicts whether a Netflix user 
will cancel their subscription using logistic regression.

## Problem Statement
Can we predict customer churn using demographic and behavioral 
features such as age, device type, subscription plan, and 
monthly spend?

## Dataset
- Source: Simulated Netflix-style customer data
- File: `users.csv`
- Size: ~10,000 records
- Features: age, gender, country, subscription_plan, 
  monthly_spend, household_size, primary_device
- Target: `is_active` (1 = active, 0 = canceled)

## Tech Stack
Python | Pandas | Scikit-learn | Seaborn | Matplotlib

## Methodology
1. Data cleaning — dropped irrelevant columns, handled nulls
2. Feature engineering — dummy variables for categorical fields
3. Train/test split — 70% train, 30% test
4. Logistic Regression model (max_iter=1000)
5. Evaluation — confusion matrix, coefficients analysis

## Results
| Metric | Score |
|--------|-------|
| Accuracy | 47% |
| Precision (Active) | 86% |
| Recall (Active) | 46% |
| F1-score | 0.60 |

## Key Findings
- Laptop and Smart TV users are more likely to stay subscribed
- Premium plan subscribers show higher churn risk
- Mobile device users have the highest cancellation rate
- Class imbalance (86% active vs 14% canceled) affected recall

## Limitations & Next Steps
- Dataset is imbalanced — apply SMOTE or class_weight balancing
- Add behavioral features: watch time, days since last login, 
  clicks per session
- Try Random Forest or XGBoost for better performance

## Context
Final project for Statistical Methods course
