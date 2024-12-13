# Customer Churn Prediction

This project aims to predict customer churn for a telecom company based on customer information, including demographics, 
account details, and service usage. The dataset contains data on various factors such as whether customers have a partner, dependents, tenure, phone service, and internet service.

## Project Overview

The project involves predicting whether a customer will churn (leave the service) based on several features.
The dataset is processed and transformed for use in machine learning models. The goal is to build an effective classification model to predict churn, which is a critical business problem for telecom companies.

## Dataset

The dataset contains 7,043 rows and 21 columns. The key columns are:
- `customerID`: Unique identifier for each customer.
- `gender`: Gender of the customer.
- `SeniorCitizen`: Whether the customer is a senior citizen (1 = Yes, 0 = No).
- `Partner`: Whether the customer has a partner.
- `Dependents`: Whether the customer has dependents.
- `tenure`: The number of months the customer has stayed with the company.
- `PhoneService`: Whether the customer has phone service.
- `MultipleLines`: Whether the customer has multiple phone lines.
- `InternetService`: Type of internet service (DSL, Fiber optic, None).
- `OnlineSecurity`, `OnlineBackup`, `DeviceProtection`, `TechSupport`: Whether the customer has these services.
- `StreamingTV`, `StreamingMovies`: Whether the customer uses streaming services.
- `Contract`: Type of contract (Month-to-month, One year, Two year).
- `PaperlessBilling`: Whether the customer has paperless billing.
- `PaymentMethod`: The payment method used by the customer.
- `MonthlyCharges`: The monthly amount billed to the customer.
- `TotalCharges`: Total amount charged to the customer.
- `Churn`: Whether the customer has churned (Yes/No).

## Data Preprocessing

The following steps were performed to prepare the dataset for model training:
1. **Handle Missing Values**: Checked for missing values and imputed or removed any entries that caused issues.
2. **Convert Categorical Features**: Converted categorical features (e.g., `gender`, `Partner`, `Churn`) into numerical values using label encoding or one-hot encoding.
3. **Handle `TotalCharges`**: Converted the `TotalCharges` column from an object type to numeric, replacing any non-numeric entries with NaN, and then filling them with appropriate values.
4. **Feature Scaling**: Scaled numerical features like `MonthlyCharges` and `tenure` to ensure that the model performs optimally.
5. **Target Variable Encoding**: The target variable `Churn` was encoded into binary values: `0` for "No" and `1` for "Yes".

## Model Development

In this project, we tested several machine learning models to predict customer churn:
- Logistic Regression
- Random Forest
- Gradient Boosting (e.g., XGBoost, LightGBM)

### Model Evaluation
Models were evaluated using several metrics:
- **Accuracy**: The percentage of correct predictions.
- **Precision**: The proportion of positive predictions that are actually correct.
- **Recall**: The proportion of actual positives correctly predicted by the model.
- **F1-Score**: The harmonic mean of precision and recall, used for imbalanced classes.
- **ROC-AUC**: The area under the Receiver Operating Characteristic curve.


