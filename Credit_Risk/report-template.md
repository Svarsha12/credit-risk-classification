# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of analysis is to check lending risk.

* Explain what financial information the data was on, and what you needed to predict.
The financial information the data was on loan lending, we needed to predict loan status.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The basic information about the variables trying to predict is loan status. The loan status count for healthy loan is 75036 and high risk loans count is 2500.

* Describe the stages of the machine learning process you went through as part of this analysis.
I created a logistic regression model with original data. In step 1 I Split the data using train_test_split and assign a random_state parameter of 1 to the model, and fit the logistic regression model using training data. Step 2 made a prediction using the testing data.
And step 3 evaluated the model performance by genarating confusion matrix and classification report.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

I used 'LogisticRegression' method. A logistic regression model is a statistical model that is used for binary classification tasks, where the goal is to predict a binary outcome—typically labeled as 0 or 1, True or False, etc. It's a type of regression analysis used when the dependent variable is categorical.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

1. Accuracy: This measures the overall correctness of the model and is 0.99.
2. Precision: for 1 (high-risk loan): This measures the proportion of positive identifications that were actually correct and for 1=0.85, 0=1.00
3. Recall for 1 (high-risk loan): This measures the ability of the model to find all positive samples (high-risk loans) for 1= 0.91 0=0.99
4. F1-Score for 1: This is the harmonic mean of precision and recall, providing a balance between the two for 1=0.88 and 0=1.00

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

Looking at the classification report and confusion matrix the logistic model prediction:

True Negative (TN): The  logistic regression model correctly predicted 'healthy loan' 18,663 times.

False Positive (FP): The logistic regression model incorrectly predicted 'high-risk loan' when it was actually 'healthy loan' 102 times.

False Negative (FN): The logistic regressionmodel incorrectly predicted 'healthy loan' when it was actually 'high-risk loan' 56 times.

True Positive (TP): The logistic regression model correctly predicted 'high-risk loan' 563 times. 

Overall, the logistic regression model performs very well in predicting both healthy loans ('o') and high risk loans('1'). It has high accuracy, good precision. Therefore, I would recommend logistic regression model.