# AR_decision_tree

I created a decision tree model in order to predict aging bucket of invoice. The goal was to predict aging bucket of invoice in order to determine which accounts needed immediate attention from account managers. The dataset was provided by the client and consisted of over 2.7 million rows and 97 columns. I calculated a new variable, age bucket, to use as the target variable for the model. The model predicts at 89% accuracy and has an error rate of 0.20. 

Multiple functions make up this code. They are explained below.

prepareData():
- Function to prepare data for analysis
- Create subsample of data - easier for processing
- Calculate age of invoice and add column to dataset (set >= 0)
- Filter data to 'Invoice' type
- Create age buckets and add column to dataset

plotDecisionTree():
- Function to train decision tree
- Create training data (70% of total) and testing data (30% of total)
- Plot decision tree
- Predict on testing data
- Print confusion matrix and calculate accuracy
- Calculate error

plotVarImp():
- Function to plot importance of variables in decision tree model

# To Run:
You must have the following R libraries installed: readr, ggplot2, dplyr, lubridate, rpart, rattle, rpart.plot, RColorBrewer, tidyverse.
