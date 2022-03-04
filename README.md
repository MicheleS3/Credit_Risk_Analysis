# Credit_Risk_Analysis

## Overview

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. We will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using credit card dataset from LendingClub, we will over and under sample data using RandomOverSampler, SMOTE, and ClusterCentroids algorithms.  Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

We will evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk.

## Results

### Random Over Sampler

![RandomOverSampler](https://user-images.githubusercontent.com/89753083/156812122-8eaab5ca-50be-4064-8765-ab1453112b5b.PNG)

The balanced accuracy score is 62.5%.
The high_risk precision is about 1%, 100% precision low_risk, 60% recall high_risk, and 65% recall low_risk.

### SMOTE

![SMOTE](https://user-images.githubusercontent.com/89753083/156812898-b1c30c1c-a66d-40c3-b216-6ae04b22407f.PNG)

The balanced accuracy score is 62.5%.
The high_risk precision is about 1%, 100% precision low_risk, 60% recall high_risk, and 65% recall low_risk.

### Cluster Centroids

![ClusterCentroids](https://user-images.githubusercontent.com/89753083/156813446-edced862-17d1-4c30-93a4-f6f78d827a1e.PNG)

The balanced accuracy score is 62.5%.
The high_risk precision is about 1%, 100% precision low_risk, 59% recall high_risk, and 43% recall low_risk.

### SMOTEENN

![SMOTEENN](https://user-images.githubusercontent.com/89753083/156813655-43bdbbf0-9e0d-43dd-b4e4-3f54a8181b67.PNG)

The balanced accuracy score is 51%.
The high_risk precision is about 1%, 100% precision low_risk, 70% recall high_risk, and 57% recall low_risk.

### Balanced Random Forest Classifier

![BalancedRandomForestClassifier](https://user-images.githubusercontent.com/89753083/156813914-fb097178-0dda-4eb0-8e42-be6a2c592fbe.PNG)

The balanced accuracy score is 78.8%.
The high_risk precision is about 4%, 100% precision low_risk, 67% recall high_risk, and 91% recall low_risk.

### Easy Ensemble Classifier

![EasyEnsembleClassifier](https://user-images.githubusercontent.com/89753083/156814177-e29d5e61-9d62-438e-b28c-1c7f61a6b989.PNG)

The balanced accuracy score is 92.5%.
The high_risk precision is about 7%, 100% precision low_risk, 91% recall high_risk, and 94% recall low_risk.

## Summary

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.  The Ensemble models had a more balanced mix of precision and recall accuracy scores.  I would recommend using the Easy Ensemble Classifier to assess credit risk.
