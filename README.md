# credit-risk-classification
# Module 12 

## Overview of the Analysis

The purpose of this analysis was to develop a machine learning model capable of assessing the credit risk associated with borrowers, based on historical lending data from a peer-to-peer lending platform. Specifically, the goal was to predict whether a loan is likely to default (high risk) or remain healthy, using a variety of borrower financial attributes.

The dataset includes financial information such as:
* Loan size
* Interest rate
* Borrower income
* Debt-to-income ratio
* Number of existing accounts
* Derogatory marks
* Total debt

The target variable is loan_status, where:
* 0 represents a healthy loan
* 1 represents a high-risk (likely to default) loan

The stages of the machine learning pipeline included:
* Loading and preprocessing the dataset
* Separating the features (X) and target labels (y)
* Splitting the data into training and testing sets
* Training a logistic regression model
* Evaluating the model’s accuracy, precision, recall, and generating a classification report

The LogisticRegression algorithm from Scikit-learn was selected due to its simplicity, interpretability, and effectiveness for binary classification problems such as credit risk analysis.

## Results

* Machine Learning Model 1: Logistic Regression
* Accuracy: 0.99
* Precision (for high-risk loans, class 1): 0.84
* Recall (for high-risk loans, class 1): 0.94

## Summary

The logistic regression model achieved an exceptionally high accuracy score of 0.99, meaning that 99% of all loan predictions were correct. More importantly, it attained a precision score of 0.84 and a recall score of 0.94 for high-risk loans (1), which are critical metrics in this context.
*Precision tells us that 84% of loans predicted to be high risk were high risk.
*Recall indicates that 94% of actual high-risk loans were correctly identified by the model.
This is especially valuable in credit risk analysis, where recall is often more important than precision. Failing to identify a high-risk borrower could lead to significant financial losses. The slightly lower precision is an acceptable trade-off if it helps ensure that most risky loans are flagged.

Based on the strong overall performance and the high recall rate, I recommend using this logistic regression model to support credit risk evaluation. It offers a reliable way to identify potentially defaulting loans, helping lenders make more informed and cautious lending decisions.
