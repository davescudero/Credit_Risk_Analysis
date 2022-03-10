# Module 17 |  Credit Risk Analysis


## Overview

For analysis we created a supervised machine learning model to accurately predict credit risk, so we created 6 different methods:

- Naive Random Oversampling
- SMOTE Oversampling
- Cluster Centroid Undersampling
- SMOTEENN Sampling
- Balanced Random Forest Classifying
- Easy Ensemble Classifying

For these different modeles we had to follow the same steps: split the data into training and testing datasets, compiled accuracy scores, confusion matries, and classification reports as my results.

## Results

### Naive Random Oversampling

- Accuracy Score: 66.7%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 68%
- Recall Low Risk: 66%
![Naive_Random_Oversampling.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling.png)

### SMOTE Oversampling

- Accuracy Score: 66.7%
- Precision High Risk: 1%
- Precision Low Risk: 100%
- Recall High Risk: 62%
- Recall Low Risk: 72%
![smote_oversampling.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/smote_oversampling.png)

## Cluster Centroid Undersampling

Accuracy Score: 51.3%
Precision High Risk: 0%
Precision Low Risk: 100%
Recall High Risk: 58%
Recall Low Risk: 44%
![undersampling.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/undersampling.png)

## SMOTEENN Sampling (Combination, over and under)

Accuracy Score: 68%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 76%
Recall Low Risk: 60%
![smoteen.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/smoteen.png)

## Balanced Random Forest Classifying

Accuracy Score: 64.8%
Precision High Risk: 56%
Precision Low Risk: 100%
Recall High Risk: 30%
Recall Low Risk: 100%
![random_forest.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/random_forest.png)

## Easy Ensemble Classifying

Accuracy Score: 93.1%
Precision High Risk: 9%
Precision Low Risk: 100%
Recall High Risk: 94%
Recall Low Risk: 92%
![easy_ensamble.png](https://github.com/davescudero/Credit_Risk_Analysis/blob/main/Resources/easy_ensamble.png)

## Summary

We are trying to find the best model which lets the least amount of high risk loans pass through undetected. The ones with the best results are:

- Easy Ensemble Classifying (93.1%)
- SMOTEENN Sampling (76%)
- Naive Random Oversampling (68%)

Another important stat to have in mind is "Recall rate for low risk" as it shows how many low risk loans are flagged as high risk. The ones that scored the highest were:

- Balanced Random Forest Classifying (100%)
- Easy Ensemble Classifying (92%)

Finally we have to look at the accuracy:

Easy Ensemble Classify (93.1%)
SMOTEENN Sampling (68%)

With all these feautures we recommend to use the **Easy Ensemble Classify Model**.
