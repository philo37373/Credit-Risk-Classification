# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Answer: The goal of this investigation is to create a model that can determine a borrower's creditworthiness. An organization that provides peer-to-peer lending services provided a record of previous loan activities. The "loan status," which indicates whether a loan is healthy or at risk, was the dependent variable (y value) in this study. Loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and negative marks were independent variables (x values). First, we divided the data into training and test sets for this study. the dependent and independent variables that we will be using. Our original data is then fitted to a logistic regression model that we have created. To create predictions, trained models are employed. Finally, we assess the model's effectiveness.In order to understand the imbalances, two distinct Logistic Regression models were produced utilizing the original data set and a randomly oversampled data set. The findings, which were acquired using the scikit-learn toolkit, were then compared. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  See credit_risk_classification file for results.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  See credit_risk_classification file for results.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Answer: According to analysis, the data gathered may be utilized to test and train the machine learning classification model. Solving the imbalance sampling problem is necessary for improved predictions. We are able to achieve higher balanced accuracy and recall scores by randomly oversampling the data. A model's ability to forecast problematic loans is improved by a greater recall value. There are two problems with inaccurate predictions. First, false positives occur when users are reported as hazardous even though they are in fact healthy, while false negatives occur when users are not flagged as risky even though they are. Each case has its expenses. It's crucial to anticipate both 1s and 0s. As a result, the model should be accurate in both respects. 