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

![RandomOverSampler - Balanced Accuracy Score](https://user-images.githubusercontent.com/104873181/188028207-d988c360-bf46-42ea-9468-195a2e8008a3.png)

![RandomOverSampler - Confusion Matrix](https://user-images.githubusercontent.com/104873181/188028226-3220e491-88f0-401f-a952-c64369ca613c.png)

![RandomOverSampler - Imbalanced Classification Report](https://user-images.githubusercontent.com/104873181/188028233-c1c0b0a3-b0f3-48c5-a52a-608e5ff1aa95.png)

### SMOTE Oversampling

![Smote Model - Balanced Accuracy Score](https://user-images.githubusercontent.com/104873181/188028290-135a6f10-833a-418b-a8b4-7579cb3bea11.png)

![Smote Model - Confusion Matrix](https://user-images.githubusercontent.com/104873181/188028308-2707f0b7-62d0-4634-8006-e82adf55cd9b.png)

![Smote Model - Imbalanced Classification Report](https://user-images.githubusercontent.com/104873181/188028318-28af31b7-adc5-43b7-bbbd-710cfb970b1b.png)

### Cluster Centroids Undersampling

![Cluster Centroids Undersampling Results](https://user-images.githubusercontent.com/104873181/188028382-6e17aac5-6b6d-4f81-ad81-1ffe3dea7322.png)

### SMOTEENN (Combination of Over and Undersampling) 

![Smoteenn - Over and Under Sampling Results](https://user-images.githubusercontent.com/104873181/188028461-3173ffb7-15c8-4335-bc3f-346d28914917.png)

### Balanced Random Forest Classifier

![Balanced Random Forest Classifier - Results](https://user-images.githubusercontent.com/104873181/188028503-4611a559-c0f6-400c-a791-9b5ec147aa66.png)

### Easy Ensemble AdaBoost Classifier

![Cluster Centroids Undersampling Results](https://user-images.githubusercontent.com/104873181/188028574-80ded517-c497-432e-b41c-02dce28a3bae.png)



