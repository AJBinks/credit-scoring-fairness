# Credit Scoring Fairness & Bias Mitigation (Reweighing)

This project demonstrates how algorithmic bias can appear in credit scoring models and how fairness techniques can be used to reduce group disparities.

## Problem

Credit scoring models may unintentionally treat certain groups unfairly due to patterns in historical data. This project evaluates fairness and applies bias mitigation.

## Approach

1. Load and clean datasets (handle missing values)
2. Train a **baseline Logistic Regression** model
3. Evaluate model performance (Accuracy, Precision, Recall, F1-score)
4. Treat **OCCUPATION_TYPE** as the sensitive attribute
5. Apply **Reweighing (bias mitigation)** using fairness sample weights
6. Compare fairness before vs after mitigation

## Fairness Metrics

* **Demographic Parity Gap (DP Gap):** difference in prediction rates across groups
* **Equal Opportunity Difference (EOD Gap):** difference in true positive rates across groups

Lower is better (closer to 0 = more fair).

## Tools

* Python
* pandas, numpy
* scikit-learn
* matplotlib

## Notes

Dataset files are not included in this repository. The notebook/script assumes pre-split training/test CSV files such as:

* X_train.csv / X_test.csv
* y_train.csv / y_test.csv

## Author

**Abdul-Jaleel Binks**
