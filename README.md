# Credit Risk Analysis

## Analysis Overview

The purpose of this analysis was to sample data from the LendingClub credit card credit dataset and create models to predict credit risk. We used the random oversampling, SMOTE oversampling, ClusterCentroid undersampling, and SMOTEEN combined sampling algorithms along with the ensemble algorithms Balanced Random Forest and Adaboost. We utilized these machine learning algorithms through the scikit-learn and imbalanced-learn libraries to build, fit, and evaluate our models sequentially using resampling. We evaluated performance of each model using confusion matrices and classification reports. 

## Results

### Non-Aggregate Algorithms


#### Random Oversampling

* Accuracy Score: 0.58
* Precision low for high- risk loans and high for low-risk loans
* High-risk recall: 0.71 // Low-risk recall: 0.58

Random Oversampling                                |   SMOTE Oversampling
:-------------------------------------------------:|:-----------------------------:
![rand_OS](https://user-images.githubusercontent.com/108199140/198361205-76f4419f-2f9e-43dc-af4a-01155825991c.PNG) |



















