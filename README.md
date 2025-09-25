# Fraud-Detection-End-to-End-Machine-Learning-Project
## Project Overview
This project demonstrates an end-to-end machine learning solution for detecting fraudulent financial transactions. Using a dataset of over **6.3 million transactions**, the goal was to accurately identify fraudulent activities while minimizing false alarms.

The project covers:
- Data cleaning and preprocessing
- Feature engineering
- Handling class imbalance
- Model training and evaluation
- Feature importance analysis
- Business insights and actionable recommendations

## Dataset
> **Note:** The dataset is not included in this repository due to size and privacy.  
To run the code, provide your own CSV file with the following columns:  
`step, type, amount, nameOrig, oldbalanceOrg, newbalanceOrig, nameDest, oldbalanceDest, newbalanceDest, isFraud, isFlaggedFraud`.

## Key Features & Models
- Handled categorical features (`type`) with one-hot encoding
- Engineered balance difference features (`errorBalanceOrig`, `errorBalanceDest`) for fraud detection
- Handled extreme class imbalance using class weights
- Models used:
  - Logistic Regression (baseline)
  - Random Forest (final model with top performance)

## Performance
- Random Forest achieved near-perfect precision and recall for fraud detection
- ROC-AUC: 0.9997
- Key features driving fraud: balance discrepancies and certain transaction types
