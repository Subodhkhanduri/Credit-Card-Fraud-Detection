# Credit-Card-Fraud-Detection
Dataset Description 
Source: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud (European cardholders' transactions from September 2013).
Size: 284,807 transactions (492 frauds).

Features:
30 total (V1 to V28 are PCA components + 'Time' + 'Amount').
'Class' is the target (1 = Fraud, 0 = Non-Fraud).
Challenge: Highly imbalanced dataset (fraud ≈ 0.172%).

Methodology
Data Preprocessing:
Standardization of 'Amount' and 'Time' features.
Handling of class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

Feature Engineering:
Feature scaling (StandardScaler)
No domain-specific features due to PCA anonymity.

Model Development:

Models Used:
Random Forest Classifier
XGBoost Classifier
Logistic Regression

Hyperparameter Tuning using GridSearchCV.
5-Fold Stratified Cross-Validation for model evaluation.

Evaluation Metrics:
ROC-AUC Score
Precision-Recall AUC
Confusion Matrix
F1-Score

🏆 Results

Model	ROC-AUC (CV Avg)	PR-AUC (CV Avg)
Random Forest	0.9999	0.9999

XGBoost	0.9999	0.9999

Logistic Regression	0.9955	0.9958

Final Selected Model: Random Forest Classifier

Performance:

High precision and recall balance.
ROC-AUC and PR-AUC close to 1.0 indicating excellent fraud detection performance.

