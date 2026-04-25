# Credit Card Fraud Detection

Financial institutions lose billions annually to credit card fraud. This project builds an end-to-end machine learning pipeline to automatically detect fraudulent transactions using a real banking dataset of 284,807 transactions.

![Python](https://img.shields.io/badge/Python-3.12-blue) ![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange) ![Status](https://img.shields.io/badge/Status-Complete-green)

---

## What I Built

A complete fraud detection pipeline covering data exploration, visualisation, class imbalance handling, model training, and business impact quantification. Two models were trained and compared: Logistic Regression and Random Forest.

---

## Dataset

- Source: Kaggle - ULB Machine Learning Group (Credit Card Fraud Detection)
- 284,807 transactions from European cardholders
- Only 492 fraudulent transactions (0.17%) - a heavily imbalanced real-world problem
- 28 PCA-anonymised features plus Amount and Time

---

## Results

| Model | Precision | Recall | F1 Score | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression | 0.06 | 0.92 | 0.11 | 0.9668 |
| Random Forest | 0.87 | 0.83 | 0.85 | 0.9731 |

Random Forest was selected as the final model based on its superior precision and F1 score. High precision is critical in banking to avoid flagging legitimate customer transactions.

---

## Business Impact

Evaluated on 56,962 held-out transactions:

- Fraud cases detected: 81 out of 98 (82.7%)
- Estimated value protected: $9,899
- Estimated value at risk from missed fraud: $2,078
- ROC-AUC: 0.9731

---

## Key Steps

1. Loaded and explored the dataset - checked class distribution, nulls, and statistical summaries
2. Visualised fraud patterns by transaction amount and hour of day
3. Applied SMOTE to handle the 99.83% vs 0.17% class imbalance
4. Trained Logistic Regression and Random Forest classifiers
5. Evaluated using Confusion Matrix, ROC Curve, Precision, Recall, and F1
6. Translated model output into a business impact report

---

## Tools and Libraries

Python, pandas, NumPy, scikit-learn, imbalanced-learn, matplotlib, seaborn, Jupyter Notebook

---

## Project Structure
fraud-detection-portfolio/
        notebooks/
            fraud_detection_analysis.ipynb
        visuals/
            01_class_distribution.png
            02_amount_analysis.png
            03_fraud_by_hour.png
            04_correlation_heatmap.png
            05_top_features.png
            06_confusion_matrices.png
            07_roc_curve.png
            08_feature_importance.png
            09_executive_summary.png
        README.md
---

## How to Run

1. Download the dataset from Kaggle: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
2. Place `creditcard.csv` in the root folder
3. Open `notebooks/fraud_detection_analysis.ipynb` in Jupyter
4. Run all cells in order
