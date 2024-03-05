# credit-risk-classification

### 
In this challenge, will use various techniques to train and evaluate a model based on loan risk.  Will use a dataset of historical lending activity from peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.  

# Overview of the Analysis 

### Factors considered in the analysis included data on: 
 1) loan size
 2) interest rate
 3) borrower's income
 4) debt to income
 5) number of accounts
 6) total debt
 7) loan status

The dataset (77,536 data points) was split into training and testing sets.   Using the original data set, created an initial logistic regression model using sklearn - model 1.  The purpose of logistic regression model is to predict both the 0 (healthy loan) and 1 (high-risk loan) labels. 

This intial model was drawing from a dataset that had 75,036 healthy loans and 2500 high-risk loans.  To resample the training data and ensure the logistic regression model had an equal number of data points, the training set data was resampled with RandomOverSampler module.  This generated 56,277 data points for both healthy loans (0) and high-risk loans (1) from the original data set. 

The resampled data was used on a new logistic regression model - model 2.   This will determine whether a loan to the borrower in the testing set would be low or high risk.  

# Results

### 
Model 1 - the logistic regression model predicted a healthy, low-risk loan with 100% precision.  It predicted a high-risk loan with lower precision at 87%.  The balance accuracy of the model is 97%. 

Model 2 - the resampled logistic regression model predicted a healthy, low-risk loan with 100% precision.  It predicts a high-risk loan with lower precision at 87%.  The balance accuracy of the model is 100%. 

# Summary

###

Model 2 had a better prediction with a higher accuracy rate.   Model 2 would be the preferred method.   

