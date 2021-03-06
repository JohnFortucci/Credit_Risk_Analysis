# Credit Risk Analysis

## Introduction

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. By employing different techniques to train and evaluate models with unbalanced classes. 

You have been asked to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 

Use a combinatorial approach of over and undersampling using the SMOTEENN algorithm. 

Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

Evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Deliverable 1 and 2 - Use Resampling Models to Predict Credit Risk

### Overview

Using imbalanced-learn and scikit-learn libraries, evaluate three machine learning models by using resampling to determine which is better at predicting credit risk. 
Use the oversampling RandomOverSampler and SMOTE algorithms, and use the undersampling ClusterCentroids algorithm. Using these algorithms resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Results

#### Naive Random Oversampling

The image below shows the output of the code execution in the Naive Random Oversampling code blocks.

![Naive Random Oversampling](/Resources/Native_Random_Oversampling.png)

From the above we can determine :- 

- Balanced Accuracy Test : 67%
- Precision for high risk : 1% , which indicates a low positivitey
- Recall for high risk    : 74%

#### SMOTE Oversampling

The image below shows the output of the code execution in the SMOTE Oversampling code blocks.

![SMOTE Oversampling](/Resources/SMOTE_Oversampling.png)

From the above we can determine :- 

- Balanced Accuracy Test : 64%
- Precision for high risk : 1% , which indicates a low positivitey
- Overall recall          : 66%

### Undersampling

The image below shows the output of the code execution in the undersampling code blocks.

![Undersampling](/Resources/Undersampling.png)

From the above we can determine :- 

- Balanced Accuracy Test : 52%
- Precision              : 99% 
- Recall                 : 44%

### Combination (Over and Under sampling)

The image below shows the output of the code execution in the Over and Under sampling code blocks.

![Combined](/Resources/Combined.png)

- Balanced Accuracy Test : 64%
- Precision              : 99% 
- Recall                 : 56%

## Deliverable 3- Use Ensemble Classifiers to Predict Credit Risk

### Overview

Using the imblearn.ensemble library, train and compare two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluate each model. 

Using both algorithms, resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

### Results

#### Balanced Random Forrest Classifier

The image below shows the output of the code execution in the random forrest code blocks.

![Balanced Random Forrest](/Resources/RandomForrest.png)

- Balanced Accuracy Test : 79%
- Precision              : 99% 
- Recall                 : 91%

#### Easy Ensemble

The image below shows the output of the code execution in the easy ensemble code blocks.

![Easy Ensemble](/Resources/EasyEnsemble.png)

- Balanced Accuracy Test : 93%
- Precision              : 99% 
- Recall                 : 94%

### Summary

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. 

The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. 

In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well.

It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.

In your models you look for a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models , and specifically the easy ensemble. 
