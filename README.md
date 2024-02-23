# credit-risk-classification

## Overview of the Analysis

The purpose of this analysis was to use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the likelihood a loan is health or high-risk.

The dataset consists of 77,536 rows, with one target and 7 variables. The target of the model is Loan_Status, or whether a borrower's request for a loan will be approved or not. The dataset we're using skews heavily towards 0 (75,036) over 1 (2500).

Factors considered for this analysis included:
- the size of the loan
- its interest rate
- the borrower's income
- the debt to income ratio
- the number of accounts the borrower held
- derogatory marks against the borrower
- the borrower's total debt

Steps:
1) Fit a logistic regression model by using the training data (X_train and y_train) using the LogisticRegression module from scikit-learn..

2) Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

3) Evaluate the model’s performance by generating a confusion matrix, and printing a classification report.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Logistic Regression Model:
  * Accuracy: 99%
  * Precision: the model predicted Healthy Loans (0) with 100% precision, but only reached 87% precision for High-Risk Loans(1).
  * Recall: the model predicted Healthy Loans (0) with 100% recall, but only reached a recall of 89% for High-Risk Loans(1).


## Summary

Given the results listed above, I would recommend this model for predicting the risk of new loans. With combined precision and recall scores over 90%, this is a fairly good model.