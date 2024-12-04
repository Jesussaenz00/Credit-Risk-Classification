# Module 12 Report Template

## Overview of the Analysis

In this analysis, we developed a logistic regression machine learning model to predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending platform. The goal was to evaluate the risk of each loan application, enabling the company to classify loans as either high-risk (1) or healthy (0).

Dataset Overview
The dataset included financial and demographic details for each loan, with the target variable, loan_status, defined as follows:

0: Healthy loan (low-risk)
1: High-risk loan

An initial examination of the data using value_counts revealed an imbalance in the loan_status variable, with significantly more healthy loans than high-risk ones. This imbalance posed a potential challenge, as it could bias the model toward the majority class.

Machine Learning Process
Data Preparation:
Separated the data into features (X) and labels (y) with loan_status as the target variable.
Data Splitting:
Divided the dataset into training (80%) and testing (20%) subsets using train_test_split to ensure the model could generalize to new data.
Model Selection and Training:
Selected logistic regression as the algorithm due to its suitability for binary classification tasks.
Initialized the model with random_state=1 for consistent results and trained it using the training data.
Model Evaluation:
Assessed the model's performance on the test set by comparing predictions to actual values.
Utilized a confusion matrix and classification report to analyze metrics such as accuracy, precision, recall, and F1-score, providing a comprehensive evaluation of the model’s effectiveness.

## Results

Machine Learning Model 1 (Logistic Regression):

	•	Accuracy: 99%
	•	Precision for 0 (healthy loan): 1.00
	•	Recall for 0 (healthy loan): 1.00
	•	F1-Score for 0 (healthy loan): 1.00
	•	Precision for 1 (high-risk loan): 0.86
	•	Recall for 1 (high-risk loan): 0.91
	•	F1-Score for 1 (high-risk loan): 0.88

## Summary

This analysis demonstrates how logistic regression can be applied to predict loan creditworthiness. While the model performed well, attention must be given to the impact of class imbalance on its predictions to ensure fair and accurate results across both high-risk and healthy loan categories.
