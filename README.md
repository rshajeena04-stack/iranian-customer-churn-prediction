# Iranian Customer Churn Prediction

## Project Overview

This project uses machine learning to predict whether a telecom customer is likely to **churn (leave the service)**.

The project uses the **Iranian Churn Dataset** from the UCI Machine Learning Repository.

## Objective

The main objective is to identify customers who are at risk of leaving so that a telecom company can take preventive customer-retention actions.

## Dataset

- **Records:** 3,150 customers
- **Features:** 13
- **Target:** Churn
- **Churn = 0:** Customer stayed
- **Churn = 1:** Customer churned
- **Missing values:** None

### Main Features

- Call Failure
- Complaints
- Subscription Length
- Charge Amount
- Seconds of Use
- Frequency of Use
- Frequency of SMS
- Distinct Called Numbers
- Age Group
- Tariff Plan
- Status
- Age
- Customer Value

## Machine Learning Models

Three classification models were trained and compared:

1. **Logistic Regression** — baseline classification model
2. **Random Forest** — ensemble tree-based model
3. **XGBoost** — gradient boosting model

## Model Comparison

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 89.68% | 84.00% | 42.42% | 56.38% | 92.08% |
| Random Forest | 96.51% | 92.31% | 84.85% | 88.42% | 98.77% |
| XGBoost | **96.51%** | 88.89% | **88.89%** | **88.89%** | **98.97%** |

## Best Model

**XGBoost** was selected as the final model because it achieved:

- **Accuracy:** 96.51%
- **Precision:** 88.89%
- **Recall:** 88.89%
- **F1 Score:** 88.89%
- **ROC-AUC:** 98.97%

The model provides a strong balance between correctly identifying churned customers and avoiding incorrect churn predictions.

## Feature Importance

The XGBoost model identified the following features as important contributors to prediction:

1. Status
2. Complaints
3. Seconds of Use
4. Subscription Length
5. Distinct Called Numbers
6. Call Failure
7. Frequency of Use
8. Customer Value
9. Age Group
10. Frequency of SMS
11. Charge Amount
12. Tariff Plan
13. Age

## Prediction Example

The trained XGBoost model can predict both:

- **Churn prediction**
- **Churn probability**

Example:

```text
Predicted Churn: 0
Churn Probability: 13.3%
```

This means the model predicts that the customer is likely to **stay**, with an estimated churn probability of **13.3%**.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

## Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Inspection & Cleaning
   ↓
Exploratory Data Analysis
   ↓
Correlation Analysis
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Feature Importance
   ↓
Customer Churn Prediction
```

## Project Files

```text
iranian-customer-churn-prediction/
│
├── Iranian_Customer_Churn_Prediction.ipynb
├── iranian_churn_dataset.csv
├── README.md
└── requirements.txt
```

## Conclusion

This project demonstrates an end-to-end machine learning workflow for telecom customer churn prediction. Among the tested models, **XGBoost achieved the strongest overall performance**, making it the selected model for churn prediction.

The project can help telecom companies identify customers at higher risk of leaving and support targeted customer-retention strategies.
