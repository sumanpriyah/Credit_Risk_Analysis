# Credit_Risk_Analysis

## Overview of the analysis: 

The purpose of this analysis is to apply machine learning to solve a real-world problem :credit card risk. In this challenge we need to employ different techniques to train and evaluate models with unbalanced classes by using 
imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We will be do oversample the data using the RandomOverSampler and SMOTE algorithms, Undersample the data using the ClusterCentroids algorithm 
and then using combinatorial approach of over- and undersampling using the SMOTEENN algorithm

### Deliverables

1: Use Resampling Models to Predict Credit Risk
2: Use the SMOTEENN Algorithm to Predict Credit Risk
3: Use Ensemble Classifiers to Predict Credit Risk
4: A Written Report on the Credit Risk Analysis (README.md)

## Results: 

### Use Resampling Models to Predict Credit Risk 

### Naive Random Oversampling
Balance Accuracy Score = 63.67%
The False Negative = 33 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
The recall(sensitivity) for predicting Low Risk(1)is 0.62 and High Risk is 0.65 
The F1 score for Low Risk is 0.79 and for high risk is 0.02 as precision for High risk is low. 

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Deliverable1_Naive%20Random%20Oversampling.png)


### SMOTE Oversampling
Balance Accuracy Score = 63.03%
The False Negative = 33 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
The recall(sensitivity) for predicting Low Risk is 0.62 and High Risk is 0.64 
The F1 score for Low Risk is higher 0.78

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Del1_SMOTE%20Oversampling.png)

### Undersampling
Balance Accuracy Score = 51.60%
The False Negative = 35 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
The recall(sensitivity) for predicting Low Risk is 0.43 and High Risk is 0.60
The F1 score for low Risk is higher 0.60 and high risk is 0.01

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Del1_Undersampling.png)

### Combination (Over and Under) Sampling-SMOTEENN algorithm to Predict Credit Risk
Balance Accuracy Score = 62.48%
The False Negative = 25 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.01 
The recall(sensitivity) for predicting Low Risk is 0.54 and High Risk is 0.71
The F1 score for Low Risk is higher 0.70 and high risk is 0.02

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Del1_SMOTEENN%20algorithm.png)


### Use Ensemble Classifiers to Predict Credit Risk

### Balanced Random Forest Classifier
Balance Accuracy Score = 78.88%
The False Negative = 30 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.03 
The recall(sensitivity) for predicting Low Risk is 0.87 and High Risk is 0.70
The F1 score for Low Risk is higher 0.93 and high Risk is 0.06

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Del2_Ensemble%20Learners_BalancedRandomForest_classifier.png)

### Easy Ensemble AdaBoost Classifier
Balance Accuracy Score = 93.32%
The False Negative = 8 which means the Model predicted credit card risk as Low Risk but actually those are High risk.
The precision of prediction using this model:Low Risk(1) is 1 and High Risk(0) is 0.09
The recall(sensitivity) for predicting Low Risk is 0.94 and High Risk is 0.92
The F1 score for Low Risk is higher 0.97 and high risk is 0.16

![](https://github.com/sumanpriyah/Credit_Risk_Analysis/blob/main/Images/Del2_Ensemble%20Learners-%20Easy%20Ensemble%20AdaBoost%20Classifier.png)

## Summary: 
Out of all the above Models, Easy Ensemble AdaBoost Classifier seems to be best the Model to predict credit Risk. The Accuracy score is 95.03%. The False Negatives are only 8 it means Model predicted those low risk but those are high risk, compare to 
other models this model have lowest False Negative that way the High Risk credit wont out number the Low Risk credits. The sensitivity(Recall) for prediction low risk is 94% and High risk is also good which is 92%. The F1 score for low risk is 97%.
My recommendation is to use Ensembleclassifier to predict credit risk where chances of high risk will be caught in the model and chances of LendingClub loosing money/loan will be less. 
