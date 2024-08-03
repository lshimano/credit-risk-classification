# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
train and evaluate a model based on loan risk with historical lending activity.
* Explain what financial information the data was on, and what you needed to predict.
The financial information were based on the features of the data: loan size, interest rate, borrower income, debt income, number of accounts, derogatory marks, total debt. The category that I needed to predict is the loan status. I think there could have been additional features such as age (older/younger people could have been evaluated more carefully re how much loan and for how long). 
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
There were 77535 data for the loan status.
* Describe the stages of the machine learning process you went through as part of this analysis.
1. Import the modules.
2. Read the lending_data csv file and create its dataframe.
3. Create features from all columns except for loan status. Loan status was separated because it was the predicted variable.
4. Split the data into training and testing.
5. Import the LogisticRegression library.
6. Instantiate the Logistic Regression model.
7. Fit the model using the training data.
8. Make predictions using the features from the test data.
9. Generate accuracy using confusion matrix and classification report for the model.
10. Evaluate how well the logistic regression model predict the healthy loan and high-risk loan status.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithm).
LogisticRegression from sklearn, train_test_split from sklearn, confusion_matrix and classification_report from sklearn.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
      Based on the classification report, for precision scores, the healthy loans (0) were predicted 1.00 and high-risk loans (1) were predicted 0.87. For recall scores, the healthy loans (0) were predicted 1.00 and high-risk loans (1) were predicted 0.89. For accuracy score, it predicted 0.99.

## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
Overall, the model performed really well especially the healthy loans because for both precision and recall scores, they both predicted 100%, whereas for high-risk loans, they predicted 0.87 and 0.89, respectively.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
It is more important to predict high-risk loans because we do not want to accidentally provide someone a loan (false positive) if this someone is a high-risk.
If you do not recommend any of the models, please justify your reasoning.
I would still recommend this model but more features could be added to confirm if it should be put in use for predicting the health status of the loan.