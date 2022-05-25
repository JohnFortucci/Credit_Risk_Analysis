# Credit Risk Analysis

## Introduction

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. By employing different techniques to train and evaluate models with unbalanced classes. 

You have been asked to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 

Use a combinatorial approach of over and undersampling using the SMOTEENN algorithm. 

Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

Evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Deliverable 1 - Use Resampling Models to Predict Credit Risk

### Overview

Using imbalanced-learn and scikit-learn libraries, evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. 
Use the oversampling RandomOverSampler and SMOTE algorithms, and use the undersampling ClusterCentroids algorithm. Using these algorithms resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Results

The image below shows the output of the code execution in the Naive Random Oversampling code blocks.
