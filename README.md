# Credit_Risk_Analysis

## Overview of Project

The central goal of this project is to use machine learning to predict credit risk. Since credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans, this project requires us to employ different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, the project requires us to oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

This project consists of three technical analysis deliverables and a written report:

* Deliverable 1: Use Resampling Models to Predict Credit Risk.
* Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk.
* Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk.
* Deliverable 4: A Written Report on the Credit Risk Analysis (README.md).

## Results

### Deliverable 1: Use Resampling Models to Predict Credit Risk
* Create the training variables by converting the string values into numerical ones using the get_dummies() method.
* Create the target variables.
* Check the balance of the target variables.

Next, begin resampling the training data. First, use the oversampling RandomOverSampler and SMOTE algorithms to resample the data, then use the undersampling ClusterCentroids algorithm to resample the data. For each resampling algorithm, do the following:
* Use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
* Calculate the accuracy score of the model.
* Generate a confusion matrix.
* Print out the imbalanced classification report.

### Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
* Using the information we have provided in the starter code, resample the training data using the SMOTEENN algorithm.
* After the data is resampled, use the LogisticRegression classifier to make predictions and evaluate the model’s performance.
* Calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.

### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
* Create the training variables by converting the string values into numerical ones using the get_dummies() method.
* Create the target variables.
* Check the balance of the target variables.
* Resample the training data using the BalancedRandomForestClassifier algorithm with 100 estimators.
* After the data is resampled, calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.
* Print the feature importance sorted in descending order (from most to least important feature), along with the feature score.
* Resample the training data using the EasyEnsembleClassifier algorithm with 100 estimators.
* After the data is resampled, calculate the accuracy score of the model, generate a confusion matrix, and then print out the imbalanced classification report.

### Written Report on Credit Risk Analysis
For each machine learning model listed below, there is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models.

#### Random Over Sampler (Naive Random Oversampling)
* Balance Accuracy Score: 0.6835
* Model: Logistic Regression

<img width="308" alt="random_over_sampler1" src="https://user-images.githubusercontent.com/114960958/220499673-8ea6b308-eff9-49ab-8ef5-79d403ff0621.png">

#### SMOTE Oversampling
* Balance Accuracy Score: 0.6277
* Model: Logistic Regression

<img width="307" alt="SMOTE_oversampling" src="https://user-images.githubusercontent.com/114960958/220500148-06740c3e-d767-4f1b-992b-abd33b2da299.png">

#### Cluster Centroids
* Balance Accuracy Score: 0.5297
* Model: Logistic Regression

<img width="305" alt="Cluster_Centroids" src="https://user-images.githubusercontent.com/114960958/220500481-77d78557-6da6-4415-9ae8-04c81f2f32be.png">

#### SMOTEENN
* Balance Accuracy Score: 0.6548
* Model: Logistic Regression

<img width="307" alt="SMOTEENN" src="https://user-images.githubusercontent.com/114960958/220500581-a266f5de-effd-4199-b44e-ffdefae82dc8.png">

#### Balanced Random Forest Classifier
* Balance Accuracy Score: 0.8731
* Model: Accuracy Score

<img width="305" alt="balanced_random_forest_classifier" src="https://user-images.githubusercontent.com/114960958/220500737-daeefeb4-f6a7-4d94-8bbe-9eb1a3e123b7.png">

#### Easy Ensemble AdaBoost Classifier
* Balance Accuracy Score: 0.9424
* Model: Accuracy Score

<img width="303" alt="easy_ensemble_adaboost_classifier" src="https://user-images.githubusercontent.com/114960958/220500881-606e0cf1-6bfa-4df8-b7bf-65f5c98dc397.png">

## Summary

Summary of Results: 

<img width="788" alt="summary_table" src="https://user-images.githubusercontent.com/114960958/220500941-d62a8497-f47a-4a7b-8ead-f520b924a9a4.png">

### Recommendations

The Random Over Sampler (Naive Random Oversampling), SMOTE Oversampling, Cluster Centroids, and Cluster Centroids resulted in a low F1 score, all below 0.02. We can conclude that considering a helpful method for pondering the F1 score, a pronounced imbalance between sensitivity and accuracy will yield a low F1 score.

Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier has high results of precision (pre), recall (rec), specificity (spe), F1-score (f1), geo (Geometric Mean), Index Balanced Accuracy (iba) and support (sup) when we compared with others models.

We observe that the Easy Ensemble AdaBoost Classifier showed high results regarding the metrics for measuring the performance of imbalanced classes. Also, this model has the highest balance accuracy score with 0.9424. This means that it has the highest precision of data analysis or includes the correct forecast in Python Scikit learn, so we recommend this model.
