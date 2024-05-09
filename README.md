# Before You Begin

Create a new repository for this project called credit-risk-classification. Do not add this homework to an existing repository.
Clone the new repository to your computer.
Inside your credit-risk-classification repository, create a folder titled "Credit_Risk."
Inside the "Credit_Risk" folder, add the credit_risk_classification.ipynb and lending_data.csv files found in the "Starter_Code.zip" file.
Push your changes to GitHub.

I added my credit-risk analysis and report in the Credit_Risk file.

# Instructions

The instructions for this Challenge are divided into the following subsections:
Split the Data into Training and Testing Sets
Create a Logistic Regression Model with the Original Data
Write a Credit Risk Analysis Report

# Split the Data into Training and Testing Sets

Open the starter code notebook and use it to complete the following steps:
Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

# NOTE
A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

Split the data into training and testing datasets by using train_test_split.

# Create a Logistic Regression Model with the Original Data

Use your knowledge of logistic regression to complete the following steps:
Fit a logistic regression model by using the training data (X_train and y_train).
Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
Evaluate the model’s performance by doing the following:
Generate a confusion matrix.
Print the classification report.
Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

# Write a Credit Risk Analysis Report
# An overview of the analysis: Explain the purpose of this analysis.

The purpose of analysis is to check lending risk. The financial information the data was on loan lending, we needed to predict loan status.
The basic information about the variables trying to predict is loan status. The loan status count for healthy loan is 75036 and high risk loans count is 2500.
I created a logistic regression model with original data. In step 1 I Split the data using train_test_split and assign a random_state parameter of 1 to the model, and fit the logistic regression model using training data. Step 2 made a prediction using the testing data.
And step 3 evaluated the model performance by genarating confusion matrix and classification report.
I used 'LogisticRegression' method. A logistic regression model is a statistical model that is used for binary classification tasks, where the goal is to predict a binary outcome—typically labeled as 0 or 1, True or False, etc. 
It's a type of regression analysis used when the dependent variable is categorical.


The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

![Image 5-9-24 at 4 29 PM](https://github.com/Svarsha12/credit-risk-classification/assets/151500400/b404a789-c008-4365-9a19-a6650f125253)


1. Accuracy: This measures the overall correctness of the model and is 0.99.
2. Precision: for 1 (high-risk loan): This measures the proportion of positive identifications that were actually correct and for 1=0.85, 0=1.00
3. Recall for 1 (high-risk loan): This measures the ability of the model to find all positive samples (high-risk loans) for 1= 0.91 0=0.99
4. F1-Score for 1: This is the harmonic mean of precision and recall, providing a balance between the two for 1=0.88 and 0=1.00
   
A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. 
If you don’t recommend the model, justify your reasoning.

Looking at the classification report and confusion matrix the logistic model prediction:

True Negative (TN): The  logistic regression model correctly predicted 'healthy loan' 18,663 times.

False Positive (FP): The logistic regression model incorrectly predicted 'high-risk loan' when it was actually 'healthy loan' 102 times.

False Negative (FN): The logistic regressionmodel incorrectly predicted 'healthy loan' when it was actually 'high-risk loan' 56 times.

True Positive (TP): The logistic regression model correctly predicted 'high-risk loan' 563 times. 

Overall, the logistic regression model performs very well in predicting both healthy loans ('o') and high risk loans('1').
It has high accuracy, good precision. Therefore, I would recommend logistic regression model.

# Hint
I went through class materials.
