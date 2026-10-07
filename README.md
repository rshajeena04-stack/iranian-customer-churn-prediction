\# Iranian Customer Churn Prediction



\## Project Overview



This project uses machine learning to predict whether a telecom customer is likely to churn (leave the service).



The project uses the Iranian Churn Dataset from the UCI Machine Learning Repository.



\## Objective



The main objective is to identify customers who are at risk of leaving so that a telecom company can take preventive retention actions.



\## Dataset



\- Dataset: Iranian Churn Dataset

\- Records: 3,150 customers

\- Features: 13

\- Target: Churn



\## Machine Learning Models



Three classification models were tested:



1\. Logistic Regression

2\. Random Forest

3\. XGBoost



\## Results



| Model | Accuracy | Precision | Recall | F1 Score |

|---|---:|---:|---:|---:|

| Logistic Regression | 89.68% | 84.00% | 42.42% | 56.38% |

| Random Forest | 96.51% | 92.31% | 84.85% | 88.42% |

| XGBoost | 96.51% | 88.89% | 88.89% | 88.89% |



\### Best Model



\*\*XGBoost\*\*



\- Accuracy: 96.51%

\- Precision: 88.89%

\- Recall: 88.89%

\- F1 Score: 88.89%

\- ROC-AUC: 98.97%



\## Key Features



The XGBoost model identified the following as important features:



\- Status

\- Complaints

\- Seconds of Use

\- Subscription Length

\- Distinct Called Numbers

\- Call Failure

\- Frequency of Use

\- Customer Value



\## Technologies Used



\- Python

\- Pandas

\- NumPy

\- Matplotlib

\- Seaborn

\- Scikit-learn

\- XGBoost

\- Jupyter Notebook



\## Future Improvements



\- Build a web application for real-time prediction.

\- Add customer churn risk levels.

\- Provide personalized retention recommendations.

\- Deploy the model using Flask or FastAPI.

