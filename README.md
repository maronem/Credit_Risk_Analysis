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

Unfortunately, during our analysis we encountered errors that we were not able fix prior to submission. In the code files we have entered the code that would have been used to complete these analyses. Our hypothesis is that on our end we do not have a proper library version compatible with the .fit() function for imblearn. 

## Summary

While we were not able to include the ensemble reports to our analysis, we were able to compare the four non-aggregate predictive algorithms. We utilized two oversampling algorithms (Random & SMOTE), Undersampling, and the combined SMOTEEN algorithm from the Scikit-learn library. One consistency throughout all four models was that there was a high precision for low-risk loans and a very low precision for high-risk loans, showing all models are very strong at predicting true positive results for low-risk loans, but very poor positive classification for high-risk loans. Of the four models, the SMOTE oversampling and undersampling algorithms had the highest percentage of accurate predictions with the same accuracy  score of 0.659, while Random Oversampling performed slightly worse with a score of 0.581 and the SMOTEEN algorithm had the weakest prediction accuracy at 0.544. Out of the two models with the highest accuracy scores, SMOTE oversampling had the best and most balanced recall (0.68/0.63) compared to undersampling (0.40/0.69). From our model testing, we would suggest using the SMOTE oversampling algorithm to best predict credit loans. SMOTE showed the best overall recall for both low and high-risk loans and accuracy score. This being said there is a very large discrepancy in the precision for low and high risk loans. 








