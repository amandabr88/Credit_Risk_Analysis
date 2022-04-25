# Credit_Risk_Analysis

## Overview
The purpose of this analysis is to use different techniques to train and evaluate models with unbalanced classes. For this specific project.
We have used the imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

## Results

### Oversampling 
* Naive Random Oversampling
For this model, the accuracy score is 65%. Also, as we are focus on High Risk predictions,
the precision of 1% and recall of 71% is not the best model for this situation.

![Naive Random Oversampling](/Images/Naive%20Random%20Oversampling.PNG)

* SMOTE Oversampling
For this model, the accuracy score is 66%. It is a low precision model as well. (precision of 1% and recall of 63%). 

![SMOTE Oversampling](/Images/SMOTE%20Oversampling.PNG)

### Undersampling 
* Cluster Centroids
The Cluster Centroids accuracy score is low, with only 54%. Also the precision and recall remain low (pre 1% and rec 69%).

![Cluster Centroids](/Images/Undersampling.PNG)

### Combination (Over and Under) Sampling
* SMOTEEN
The SMOTEENN model still with a low accuracy score (67%). This model has a low precision (1%) when predicting 'High Risk' credits, and a not too bad recall (73%) score. However, combining the precision and recall score, this is not a good model.

![SMOTEEN](/Images/SMOTEENN.PNG)

### Ensemble Learners
* Balanced Random Forest Classifier
This model has a higher accuracy score (79%). Also, the precision score has increased to 3% and the recall is 70%, the best one so far. 

![Balanced Ransom Forecast Classifier](/Images/Balanced%20Random%20Forest%20Classifier.PNG)

* Easy Ensemble AdaBoost Classifier
This model has a very good accuracy score of 93%. The precision score now increased for 9% and recall to 92%. 
The AdaBoost model is the best one for this specific analysis. 

![Easy Ensemble AdaBoost Classifier](/Images/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

## Summary
In regard of these 6 model tested, the conclusion of this analysis is that the AddaBoost model is the most recommended for this specific dataset. As we could see above, the accuracy score for the AdaBoost model is 93%. Also, a precision of 9% and a recall of 92%.
However, the precision of 9% is not a good result. So we would recommend the user to test different model and try to get a higer precision score.
