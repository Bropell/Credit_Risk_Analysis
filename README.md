# Credit_Risk_Analysis
## Project Overview
The purpose of this project was to apply supervised machine learning techniques to solve a real-world challenge involving credit card risk. The imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling. The data was oversampled using the RandomOverSampler and SMOTE algorithms, undersampled using the ClusterCentroids algorithm, and the SMOTEENN algorithm was used for the combinatorial approach. Lastly, the aim was to reduce bias using the BalancedRandomForestClassifier and EasyEnsembleClassifier machine learning models. 

## Results
The balanced accuracy scores, precision, and recall scores are described below for each of the six machine learning models used in this analysis. For reference, the balanced 
accuracy score is a measure of how well the model predicted the actual outcome. The precision is a measure of how likely a positive value is actually true which is found by the 
following equation: Precision = (True Positives)/(True Positives + False Positives). Lastly, recall is a measure of how well a test will diagnose a correct reading, aka True
Positive or False Negative. This can be found using the following equation: Sensitivity = (True Positives)/(True Positives + False Negatives). 

<h3 align="center">Naive Random Oversampling</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Naive_Random_Oversampling.png"/>
</p><br>

- Balanced Accuracy Score: 0.646 meaning about 64.6% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.71 for high risk and .58 for low risk<br>

<h3 align="center">SMOTE Oversampling</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.png"/>
</p><br>

- Balanced Accuracy Score: 0.659 meaning about 65.9% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.63 for high risk and .68 for low risk<br>

<h3 align="center">Undersampling</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png"/>
</p><br>

- Balanced Accuracy Score: 0.544 meaning about 54.4% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.69 for high risk and .40 for low risk<br>

<h3 align="center">SMOTEENN Algorithm</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.png"/>
</p><br>

- Balanced Accuracy Score: 0.666 meaning about 66.6% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.73 for high risk and .60 for low risk<br>

<h3 align="center">Balanced Random Forest Classifier</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest.png"/>
</p><br>

- Balanced Accuracy Score: 0.789 meaning about 78.9% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.03 for high risk and 1.00 for low risk
- Recall: 0.70 for high risk and .87 for low risk<br>

<h3 align="center">Easy Ensemble Classifier</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost.png"/>
</p><br>

- Balanced Accuracy Score: 0.932 meaning about 93.2% of the observations in the testing set was predicted correctly by this model.
- Precision: 0.09 for high risk and 1.00 for low risk
- Recall: 0.92 for high risk and .94 for low risk<br>

## Summary