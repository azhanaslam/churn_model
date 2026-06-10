# Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn using the Telco Customer Churn dataset. The objective is to identify customers who are likely to leave the company and uncover the key factors influencing churn.

---

## Business Problem

Customer churn directly impacts revenue and customer lifetime value. By identifying high-risk customers in advance, businesses can take proactive retention measures and reduce customer loss.

---

## Dataset

Dataset: Telco Customer Churn

Features include:

- Customer demographics
- Account information
- Contract details
- Billing information
- Internet and support services
- Churn status (Target Variable)

Target Variable:

- Churn
  - Yes = Customer left
  - No = Customer stayed

---

## Project Workflow

### 1. Data Cleaning

- Removed customerID column
- Converted TotalCharges to numeric format
- Handled missing values

### 2. Exploratory Data Analysis (EDA)

Analyzed:

- Churn distribution
- Contract type vs churn
- Tenure vs churn
- Monthly charges vs churn
- Service adoption patterns

### 3. Feature Engineering

- Encoded target variable
- Applied One-Hot Encoding to categorical features
- Prepared dataset for machine learning

### 4. Model Building

Models trained:

1. Logistic Regression
2. Random Forest Classifier

---

## Model Performance

### Logistic Regression

| Metric | Score |
|----------|--------:|
| Accuracy | 72.8% |
| Precision | 49% |
| Recall | 80% |
| F1 Score | 61% |
| ROC-AUC | 0.836 |

### Random Forest

| Metric | Score |
|----------|--------:|
| Accuracy | 78.7% |
| Precision | 62% |
| Recall | 51% |
| F1 Score | 56% |
| ROC-AUC | 0.818 |

---

## Model Selection

Although Random Forest achieved higher accuracy, Logistic Regression delivered:

- Higher Recall
- Better ROC-AUC
- Better identification of churning customers
- Greater interpretability

For customer retention campaigns, missing a churning customer is more costly than contacting a few additional customers. Therefore, Logistic Regression was selected as the preferred model.

---

## Key Business Insights

### Factors Reducing Churn

- Two-year contracts significantly reduce churn
- One-year contracts improve retention
- Online Security reduces churn risk
- Tech Support improves customer retention
- Online Backup increases customer stickiness

### Factors Increasing Churn

- Electronic Check payment method
- Fiber Optic internet service
- Paperless Billing
- Senior Citizen customers

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Future Improvements

- Hyperparameter tuning
- XGBoost implementation
- SHAP explainability
- Streamlit deployment
- Automated churn risk dashboard

---

## Conclusion

The project successfully identified key drivers of customer churn and developed predictive models capable of detecting at-risk customers. Logistic Regression achieved the best balance between predictive performance and business interpretability, making it the preferred solution for churn prediction.
