# CustomerChrunAnalysis



# Customer Churn Prediction

This repository contains a dataset and model for predicting customer churn for a telecom company.

## Dataset Overview

The dataset contains 7,043 rows and 21 columns, including information about customer demographics, services, and account details.
The target variable is `Churn`, which indicates whether the customer has left the service.

## Data Preprocessing

The following preprocessing steps were performed:
- Encoding categorical variables (e.g., `gender`, `Contract`, `PaymentMethod`)
- Handling missing values in the `TotalCharges` column
- Feature scaling and feature engineering (optional)

## Model Development

The following models were tested:
- Logistic Regression
- Random Forest
- XGBoost

The models were evaluated using metrics like accuracy, precision, recall, and F1-score.

## How to Run the Code

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
