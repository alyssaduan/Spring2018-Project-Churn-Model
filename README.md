# Spring2018-Project-Churn-Model

In this project, we use 11 factors to predict whether a customer will churn to another company. 
Data Description:

Each row represents a customer of the network, with the parameters for each customer described below.

       The data consists of 20,000 customers, split into 90% (18,000) for training data
       The remaining 10% (2,000) as test data (holdout).

Find the labeled training data in 'train.csv' and unlabeled test data in 'test.csv'.

Features of each customer:

       COLLEGE	              Is the customer college educated?
       INCOME	Annual               income
       OVERAGE	              Average overcharges per month
       LEFTOVER	              Average number of leftover minutes per month	
       HOUSE	                     Estimated value of dwelling (from census tract)	
       HANDSET_PRICE	              Cost of phone
       OVER_15MINS_CALLS_PER_MONTH	Average number of long calls (15 mins or over) per month	
       AVERAGE_CALL_DURATION	Average duration of a call
       REPORTED_SATISFACTION	Reported level of satisfaction
       REPORTED_USAGE_LEVEL	       Self-reported usage level
       CONSIDERING_CHANGE_OF_PLAN	Whether the customer considered changing their plan	
       LEAVE (Target variable)	Did the customer stay or leave (churn)?
	

Step1: Deal with Data (Both train and test data)

       1) Catogorize Data by Using Catagory Numbers
       2) Use corr() to calculate correlation between LEAVE
       3) Separate data by their features and then hstack
       4) Use StandardScaler to normalized Data
       
Step2: Fit Model with Logistic Regression

       Use 1 degree feartures => Accurancy: 0.637
       Use polynomial features => Accurancy: 0.652
       Use 3 degree features => Accurancy: 0.673
       Increase degree to increase training data accurancy => Overfit
       
Step3: Fit Model with SVM => Accurancy: 0.698




