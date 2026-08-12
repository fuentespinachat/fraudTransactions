# fraudTransactions
# Credit Card Fraud Detection Using Machine Learning

A machine learning project that detects potentially fraudulent credit card transactions using supervised classification.

## Project Overview

This project analyzes credit card transaction data and compares different machine learning models to identify fraudulent transactions.

The dataset contains **32,300 transactions** with transaction and customer-related variables. The target variable is `is_fraud`:

* `0` = Legitimate transaction
* `1` = Fraudulent transaction

## Models Used

The following models were developed and compared:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost
* Support Vector Machine (SVM)

## Data Processing

The project includes:

* Data cleaning
* Duplicate removal
* Missing-value imputation
* Outlier and invalid-value handling
* Feature scaling
* Feature engineering
* Correlation analysis
* Random Forest feature importance
* Principal Component Analysis (PCA)

## Model Evaluation

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

The **Tuned Logistic Regression** model was selected as the final model because it provided a good balance between fraud detection performance and interpretability.

### Final Model Performance

| Metric    |  Score |
| --------- | -----: |
| Accuracy  | 74.05% |
| Precision | 73.24% |
| Recall    | 72.69% |
| F1-score  | 72.96% |
| ROC-AUC   | 81.83% |

## Explainability and Fairness

The project also used:

* SHAP
* LIME
* Partial Dependence Plots (PDP)
* Individual Conditional Expectation (ICE)
* Age-group fairness analysis

The fairness analysis identified a difference in recall between the youngest and oldest age groups, highlighting the importance of monitoring model performance across different groups.

## Files

* `Credit_Fraud.ipynb` – Main machine learning notebook
* `Credit_Fraud_Capstone_Report.docx` – Capstone project report

## Tools and Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* SHAP
* LIME
* Matplotlib
* Seaborn

## Note

This project is intended for academic and analytical purposes. The model requires further validation, including realistic fraud rates, time-based testing, and improved preprocessing, before being considered for real-world financial use.
