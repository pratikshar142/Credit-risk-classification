# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis is to create a supervised machine learning model that will predict if a loan is healthy (class 0) or high-risk (class 1). We will use logistic regression as a binary classifier for our model here.   The data used is a 77,500-line CSV file.

* Explain what financial information the data was on, and what you needed to predict.
The analysis was conducted on financial data, specifically focusing on loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The objective was to predict the loan status, either as a healthy loan (0) or a high-risk loan (1).

* Describe the stages of the machine learning process you went through as part of this analysis.
The stages of the machine learning process in this analysis included:

Splitting data into labels and features, with the loan status (healthy or high-risk) being the label and the remaining seven columns as features.
The data was then split into training and testing data sets.
A Logistic Regression model from sklearn was created.
Logistic Regression as a binary classifier was chosen as we are classifying loans as healthy OR high-risk and only those two options.
The model was then fit with the training data.
Predictions were made with the test data.
The model’s performance was evaluated using accuracy, precision, and recall scores.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
The Logistic Regression model was used to predict the values.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

Description of Logistic Regression Model Accuracy, Precision, and Recall scores.

Accuracy: The overall accuracy of the model is 0.99, indicating that it correctly classifies 99% of the instances.

Precision

Healthy Loan (class 0): 1.00
High-Risk Loan (class 1): 0.84
Recall

Healthy Loan (class 0): 0.99
High-Risk Loan (class 1): 0.94

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
While both give 99% accuracy, the f1-score and recall are better for sampled data.


* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
For trying to classify loans, trying to prevent high-risk loans is more important than giving out a loan as more money can be lost from a single loan that defaults than the interest earned from a loan


If you do not recommend any of the models, please justify your reasoning.
The Logistic regression model with balanced dataset seems to be performing good predicting the healthy loans (class 0), with precision 1.00, recall 0.99. When it comes to risky loans (class 1), the model is still doing a good prediction, precision 0.84 and recall 0.99.
