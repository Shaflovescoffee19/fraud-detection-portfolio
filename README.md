\# Credit Card Fraud Detection

\### Financial Data Analytics Portfolio Project



!\[Python](https://img.shields.io/badge/Python-3.12-blue)

!\[scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)

!\[Status](https://img.shields.io/badge/Status-Complete-green)



\## Business Problem

Financial institutions lose billions annually to credit card fraud. This project builds a machine learning pipeline to detect fraudulent transactions in real-time using a dataset of 284,807 transactions from a European bank.



\## Dataset

\- \*\*Source:\*\* Kaggle — ULB Machine Learning Group

\- \*\*Size:\*\* 284,807 transactions

\- \*\*Fraud rate:\*\* 0.17% (highly imbalanced)

\- \*\*Features:\*\* 28 PCA-anonymised features + Amount + Time



\## Key Results



| Model | Precision | Recall | F1 Score | ROC-AUC |

|---|---|---|---|---|

| Logistic Regression | 0.06 | 0.92 | 0.11 | 0.9668 |

| \*\*Random Forest\*\* | \*\*0.87\*\* | \*\*0.83\*\* | \*\*0.85\*\* | \*\*0.9731\*\* |



\## Business Impact (Test Set — 56,962 transactions)

\- Fraud cases detected: \*\*81 out of 98 (82.7%)\*\*

\- Estimated value protected: \*\*$9,899\*\*

\- Estimated value at risk: \*\*$2,078\*\*

\- ROC-AUC Score: \*\*0.9731\*\*



\## Techniques Used

\- Exploratory Data Analysis (EDA)

\- Class imbalance handling with SMOTE

\- Logistic Regression vs Random Forest comparison

\- Confusion Matrix, ROC-AUC, Precision-Recall evaluation

\- Feature importance analysis

\- Business impact quantification



\## Project Structure

fraud-detection-portfolio/

├── notebooks/

│   └── fraud\_detection\_analysis.ipynb

├── visuals/

│   ├── 01\_class\_distribution.png

│   ├── 02\_amount\_analysis.png

│   ├── 03\_fraud\_by\_hour.png

│   ├── 04\_correlation\_heatmap.png

│   ├── 05\_top\_features.png

│   ├── 06\_confusion\_matrices.png

│   ├── 07\_roc\_curve.png

│   ├── 08\_feature\_importance.png

│   └── 09\_executive\_summary.png

└── README.md

\## Author

Built as part of a Data Analyst portfolio targeting financial services roles.

