# Banking Fraud Detection: Machine Learning

Classical ML for fraud detection, built on banking use cases.

## Capstone: Credit Card Fraud Detection
Real Kaggle dataset (ULB), 284,807 transactions, 0.173% fraud.

- Compared Logistic Regression and Random Forest across three
  imbalance techniques: baseline, class weights, SMOTE
- Best model (Random Forest): Precision 0.941, Recall 0.816,
  F1 0.874, PR-AUC 0.861 on 56,962 held-out transactions
- Threshold tuning with precision-recall curves
- Model and scaler saved with joblib

## Files
| File | What it does |
|---|---|
| `fraud_analysis_capstone.ipynb` | Full pipeline on the real dataset |
| `fraud_model_final.pkl`, `scaler_final.pkl` | Saved capstone model and scaler |
| `fraud_model.ipynb` | First models on synthetic data: LR, Decision Tree, Random Forest |
| `fraud_analysis.ipynb` | Data cleaning and risk scoring with Pandas |
| `fraud_detector.py` | Rule-based fraud flags with Pandas |
| `transaction_analyzer.py` | Python module for transaction analysis |

## Dataset
Kaggle "Credit Card Fraud Detection" (mlg-ulb). Not included
because of file size. Download it and place `creditcard.csv`
next to the notebook.

## Run it
pip install -r requirements.txt
jupyter notebook

## Skills shown
Python, Pandas, NumPy, Scikit-learn, imbalanced-learn, EDA,
feature scaling, class imbalance, precision/recall/PR-AUC,
threshold tuning
