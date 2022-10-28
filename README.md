# Credit Risk Analysis

## Analysis Overview

The purpose of this analysis was to sample data from the LendingClub credit card credit dataset and create models to predict credit risk. We used the random oversampling, SMOTE oversampling, ClusterCentroid undersampling, and SMOTEEN combined sampling algorithms along with the ensemble algorithms Balanced Random Forest and Adaboost. We utilized these machine learning algorithms through the scikit-learn and imbalanced-learn libraries to build, fit, and evaluate our models sequentially using resampling. We evaluated performance of each model using confusion matrices and classification reports. 

## Results

### Non-Aggregate Algorithms

| Result          | Random Oversampling | SMOTE Oversampling  | Undersampling | SMOTEEN |
| --------------- | ------------------- | ------------------- | ------------- | ------------- |
| Accuracy Score  | 0.581               | 0.659               | 0.659         | 0.544 |
| Low-Risk Precision  | High (1.00)     | High (1.00)         | High (1.00)   | High (1.00) |
| High-Risk Precision  | Low (0.01)     | Low (0.01)          | Low (0.01)    | Low (0.01) |
| Low-Risk Recall  | 0.58               | 0.68                | 0.40          | 0.57 | 
| High-Risk Recall  | 0.71              | 0.63                | 0.69          | 0.72 | 

#### Legend:

* Accuracy score: Percentage of accurate predictions
* Precision: The number of positive class predictions that are actually positive
* Recall: The number of positive class predictions of all positive class examples

Random Oversampling                                |   SMOTE Oversampling
:-------------------------------------------------:|:-----------------------------:
![rand_OS](https://user-images.githubusercontent.com/108199140/198361205-76f4419f-2f9e-43dc-af4a-01155825991c.PNG) | ![SMOTE_OS](https://user-images.githubusercontent.com/108199140/198366717-753207cf-1938-4743-a224-333ec1a4dfda.PNG) 

Undersampling                                      |   SMOTEEN
:-------------------------------------------------:|:-----------------------------:
![LR_US](https://user-images.githubusercontent.com/108199140/198366857-da6be1ab-2ebe-4559-a6f8-5a5ba6544756.PNG) | ![Combo_OSUS](https://user-images.githubusercontent.com/108199140/198366884-f35993da-d5fd-4ff2-b9c6-70df978386b0.PNG)

### Ensemble Algorithms

Balanced Random Forest                             |   Adaboost
:-------------------------------------------------:|:-----------------------------:
![image](https://user-images.githubusercontent.com/108199140/198453402-9a8d0906-bdd1-41bb-bb36-514ad6862657.png) | ![image](https://user-images.githubusercontent.com/108199140/198453503-1e69a804-193e-431c-9220-65ca533c09a7.png)



## Summary










