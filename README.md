# 📱 Telco Customer Churn Prediction (91% Accuracy)

This repository contains an end-to-end Machine Learning pipeline designed to predict customer attrition (Churn) for a telecommunications company. By identifying high-risk customers, this project enables data-driven retention strategies.

## 🎯 Project Overview
The goal is to analyze customer behavior (contract type, tenure, charges, etc.) and build a predictive model to determine the likelihood of a customer leaving the service.



## 🛠️ Key Technical Steps

### 1. Data Preprocessing & Cleaning
* **Type Casting:** Converted `TotalCharges` from object to numeric, handling missing/empty strings.
* **Feature Engineering:** Applied **Label Encoding** to transform categorical features (Gender, Payment Method, etc.) into a machine-readable format.

### 2. Exploratory Data Analysis (EDA)
* Visualized **Churn Class Distribution** to understand the balance of the target variable.
* Generated a **Correlation Heatmap** to identify the strongest churn drivers (e.g., Monthly Charges and Contract type).



### 3. Model Development & Benchmarking
I experimented with several classification algorithms to find the best performer:
* Logistic Regression
* Random Forest
* XGBoost
* **CatBoost** (Winner 🏆)

### 📈 Final Results
The **CatBoost** model outperformed all other baselines:
* **Accuracy:** 91%
* **Key Drivers:** Contract type (Month-to-month) and Tenure were found to be the most significant predictors of churn.
