# Customer Churn Prediction

Churn prediction project using Logistic Regression.

Important observations:
Customers on two-year contracts showed the lowest likelihood of churn.
Online security and technical support services were strongly associated with customer retention.
Customers using electronic check payments exhibited higher churn rates.
Fiber optic internet users demonstrated increased churn propensity.
Additional service adoption (backup, protection, support) reduced churn risk.

AUC-ROC:
Built a customer churn prediction model using Logistic Regression on the Telco Customer Churn dataset. Achieved 72.8% accuracy, 80% recall on churn customers, and a ROC-AUC score of 0.84. Identified contract duration, online security, and technical support as major retention drivers, while electronic check payments and fiber optic service were associated with higher churn risk.

Recommended model:
Logistic Regression

Reason:
Although Random Forest achieved higher overall accuracy (78.7%), Logistic Regression achieved substantially higher recall (80% vs 51%) and a better ROC-AUC score (0.836 vs 0.818), making it more effective for identifying customers at risk of churn.
