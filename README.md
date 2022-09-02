# Credit_Risk_Analysis

## Overview

In this assignment, we will use Python to buid and evaluate different machine learning models to precict crect risk.

We will use the following procedures:
1. Oversample the data using Ramdom Over Sampler and SMOTE algorithms
2. Undersample the data using Cluster Centroids algorithm
3. Use a combinational approach over and undersampling using SMOTE-ENN algorithm
4. Compare two machine learning models that reduce biases i.e. Balanced Ramdom Forest Classifier and Easy Ensemple CLassifier

We will evaluate the performance of these models and make recomendation on whether they should be used to predict credit risk.


## Results 

We will show the Balanced Accuracy Scores, Confusion Matrix and Imbalanced Classifiers for each model.

### RandomOverSampler Model

Balanced Accuracy Score = 0.637

High Risk Precision = 1% with Sensitivity at 62%, f1 = 2%

Low Risk Precision = 100% with Sensitivity at 65%, f1 = 79%

Low risk precision of 100% with sensitivity at 65% shows high number of low risk population

![RandomOverSampler - Results](https://user-images.githubusercontent.com/104873181/188028840-5fe9db0e-84a1-4f36-bac9-64a0338c6c72.png)

### SMOTE Oversampling

Balanced Accuracy Score = 0.602

High Risk Precision = 1% with Sensitivity at 62%, f1 = 2%

Low Risk Precision = 100% with Sensitivity at 64%, f1 = 78%

Results are almost similar to RandomOverSampler

![Smote Model - Results](https://user-images.githubusercontent.com/104873181/188028856-9395fca5-2c38-4844-be15-a606fa502156.png)

### Cluster Centroids Undersampling

Balanced Accuracy Score = 0.510

High Risk Precision = 1% with Sensitivity at 59%, f1 = 1%

Low Risk Precision = 100% with Sensitivity at 43%, f1 = 60%

Due to the high number of false positives, the low_risk sensitivity is only 43%

![Cluster Centroids Undersampling Results](https://user-images.githubusercontent.com/104873181/188028382-6e17aac5-6b6d-4f81-ad81-1ffe3dea7322.png)

### SMOTEENN (Combination of Over and Undersampling) 

Balanced Accuracy Score = 0.625

High Risk Precision = 1% with Sensitivity at 71%, f1 = 2%

Low Risk Precision = 100% with Sensitivity at 54%, f1 = 70%

Due to the high number of false positives, the low_risk sensitivity is only 54%

![Smoteenn - Over and Under Sampling Results](https://user-images.githubusercontent.com/104873181/188028461-3173ffb7-15c8-4335-bc3f-346d28914917.png)

### Balanced Random Forest Classifier

Balanced Accuracy Score = 0.775

High Risk Precision = 3% with Sensitivity at 64%, f1 = 6%

Low Risk Precision = 100% with Sensitivity at 91%, f1 = 95%

Due to the low number of false positives, the low_risk sensitivity is at 91% with 100% Precision

![Balanced Random Forest Classifier - Results](https://user-images.githubusercontent.com/104873181/188028503-4611a559-c0f6-400c-a791-9b5ec147aa66.png)

### Easy Ensemble AdaBoost Classifier

Balanced Accuracy Score = 0.925

High Risk Precision = 7% with Sensitivity at 91%, f1 = 14%

Low Risk Precision = 100% with Sensitivity at 94%, f1 = 97%

Due to the low number of false positives, the low_risk sensitivity is at 94% with 100% Precision

![Cluster Centroids Undersampling Results](https://user-images.githubusercontent.com/104873181/188028574-80ded517-c497-432e-b41c-02dce28a3bae.png)

## Summary

Overall the 2 Ensemble performed better than the Oversampling/Undersampling/Combination algorithms. The worst performance was from Cluster Cenroids with a balanced accuracy score of 0.51. The best performance was from Easy Ensemble AdaBoost Classifier with a score of 0.925.

Low Risk precision score was the same accross all i.e. 100%

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The ensemble models brought a significant impovement specially on the high risk credits. The recall of 92.5% shows that the Easy Ensemble Classifier detects a high degree of high risk credits. WIth low levels of precision, the model still falsely detects low risk credits as high risk. 

In my opinion, all models have low degree of precision and will not be suitable for use. Inaccurate analysis can result in missed business opportunities and may result in regulatory issues for the bank.

