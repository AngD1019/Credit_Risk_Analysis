# Credit_Risk_Analysis

## Overview of Project

The central goal of this project is to use machine learning to predict credit risk. Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, this project requires us to employ different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the project requires us to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

This project consists of three technical analysis deliverables and a written report. You will submit the following:

Deliverable 1: Use Resampling Models to Predict Credit Risk.
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk.
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk.
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md).
Files
Use the following link to download the Challenge starter code.

Module 18 challenge starter codeLinks to an external site.
Before You Start
Create a new GitHub repository entitled "Credit_Risk_Analysis" and initialize the repository with a README.

Instructions
Deliverable 1: Use Resampling Models to Predict Credit Risk
Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm. Using these algorithms, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

Follow the instructions below and use the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 1.

Open the credit_risk_resampling_starter_code.ipynb file, rename it credit_risk_resampling.ipynb, and save it to your Credit_Risk_Analysis folder.

Using the information we’ve provided in the starter code, create your training and target variables by completing the following steps:

Create the training variables by converting the string values into numerical ones using the get_dummies() method.
Create the target variables.
Check the balance of the target variables.
Next, begin resampling the training data. First, use the oversampling RandomOverSampler and SMOTE algorithms to resample the data, then use the undersampling ClusterCentroids algorithm to resample the data. For each resampling algorithm, do the following:

Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
Calculate the accuracy score of the model.
Generate a confusion matrix.
Print out the imbalanced classification report.
Save your credit_risk_resampling.ipynb file to your Credit_Risk_Analysis folder.

Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
Using your knowledge of the imbalanced-learn and scikit-learn libraries, you’ll use a combinatorial approach of over- and undersampling with the SMOTEENN algorithm to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Using the SMOTEENN algorithm, you’ll resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

Follow the instructions below and use the information in the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 2.

Continue using your credit_risk_resampling.ipynb file where you have already created your training and target variables.
Using the information we have provided in the starter code, resample the training data using the SMOTEENN algorithm.
After the data is resampled, use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
Calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
Save your credit_risk_resampling.ipynb file to your Credit_Risk_Analysis folder.

Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Using your knowledge of the imblearn.ensemble library, you’ll train and compare two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. Using both algorithms, you’ll resample the dataset, view the count of the target classes, train the ensemble classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

Follow the instructions below and use the information in the credit_risk_resampling_starter_code.ipynb file to complete Deliverable 3.

Open the credit_risk_ensemble_starter_code.ipynb file, rename it credit_risk_ensemble.ipynb, and save it to your Credit_Risk_Analysis folder.
Using the information we have provided in the starter code, create your training and target variables by completing the following:
Create the training variables by converting the string values into numerical ones using the get_dummies() method.
Create the target variables.
Check the balance of the target variables.
Resample the training data using the BalancedRandomForestClassifier algorithm with 100 estimators.
Consult the following Random Forest documentationLinks to an external site. for an example.
After the data is resampled, calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
Print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
Next, resample the training data using the EasyEnsembleClassifier algorithm with 100 estimators.
Consult the following Easy Ensemble documentationLinks to an external site. for an example.
After the data is resampled, calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
Save your credit_risk_ensemble.ipynb file to your Credit_Risk_Analysis folder.

Deliverable 4: Written Report on the Credit Risk Analysis
For this deliverable, you’ll write a brief summary and analysis of the performance of all the machine learning models used in this Challenge.

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.

Requirements
Deliverable 1: Use Resampling Models to Predict Credit Risk (30 points)
You will earn a perfect score for Deliverable 1 by completing all requirements below:

For all three algorithms, the following have been completed:
An accuracy score for the model is calculated (7.5 pt)
A confusion matrix has been generated (7.5 pt)
An imbalanced classification report has been generated (15 pt)
Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk (15 points)
You will earn a perfect score for Deliverable 2 by completing all requirements below:

The combinatorial SMOTEENN algorithm does the following:
An accuracy score for the model is calculated (5 pt)
A confusion matrix has been generated (5 pt)
An imbalanced classification report has been generated (5 pt)
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk (25 points)
You will earn a perfect score for Deliverable 3 by completing all requirements below:

The BalancedRandomForestClassifier algorithm does the following:
An accuracy score for the model is calculated (2.5 pt)
A confusion matrix has been generated (2.5 pt)
An imbalanced classification report has been generated (5 pt)
The features are sorted in descending order by feature importance (5 pt)
The EasyEnsembleClassifier algorithm does the following:
An accuracy score of the model is calculated (2.5 pt)
A confusion matrix has been generated (2.5 pt)
An imbalanced classification report has been generated (5 pt)
Deliverable 4: Written Report on the Credit Risk Analysis (30 points)
Structure, Organization, and Formatting
The written analysis has the following structure, organization, and formatting:

There is a title, and there are multiple sections (2 pt)
Each section has a heading and subheading (2 pt)
Links to images are working, and code is formatted and displayed correctly (2 pt).
Analysis
The written analysis has the following:

Overview of the loan prediction risk analysis:

The purpose of this analysis is well defined (4 pt)
Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)
## Summary:

There is a summary of the results (2 pt)
There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
