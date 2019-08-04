# Spring2018-Project-Churn-Model

In this project, we use 11 factors to predict whether a customer will churn to another company. 


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




