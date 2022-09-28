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

- Balanced Accuracy Score: 0.646 meaning about 64.6% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.71 for high risk and .58 for low risk<br>

<h3 align="center">SMOTE Oversampling</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Oversampling.png"/>
</p><br>

- Balanced Accuracy Score: 0.659 meaning about 65.9% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.63 for high risk and .68 for low risk<br>

<h3 align="center">Undersampling</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Undersampling.png"/>
</p><br>

- Balanced Accuracy Score: 0.544 meaning about 54.4% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.69 for high risk and .40 for low risk<br>

<h3 align="center">SMOTEENN Algorithm</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.png"/>
</p><br>

- Balanced Accuracy Score: 0.666 meaning about 66.6% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.01 for high risk and 1.00 for low risk
- Recall: 0.73 for high risk and .60 for low risk<br>

<h3 align="center">Balanced Random Forest Classifier</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Balanced_Random_Forest.png"/>
</p><br>

- Balanced Accuracy Score: 0.789 meaning about 78.9% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.03 for high risk and 1.00 for low risk
- Recall: 0.70 for high risk and .87 for low risk<br>

<h3 align="center">Easy Ensemble Classifier</h3>
<p align="center">
    <img src= "https://github.com/Bropell/Credit_Risk_Analysis/blob/main/Resources/Easy_Ensemble_AdaBoost.png"/>
</p><br>

- Balanced Accuracy Score: 0.932 meaning about 93.2% of the observations in the testing set were predicted correctly by this model.
- Precision: 0.09 for high risk and 1.00 for low risk
- Recall: 0.92 for high risk and .94 for low risk<br>

## Summary
Based on the balanced accuracy score, precision and recall of each machine learning model, there are some points to be made. Each 
model had greater than a 50% balanced accuracy score which shows that none of the models were horrible at predicting the actual
outcomes. All the models were very precise regarding low-risk loans with a value of 1, which is as good as it gets. The precision
for high-risk loans, however, was very low for all the models with the highest precision value being only .09. Regarding recall,
each model displayed moderately different values for both the low-risk and high-risk loans. In the case that only one model needed to 
be used, it is strongly recommended to use the Easy Ensemble Classifier model. This model seemed to exceed all others in its performance
in every single parameter measured. It had the highest balanced accuracy score of .932 meaning about 93.2% of the observations in the
testing set were predicted correctly. Its precision for low-risk loans matched the other models with a value of 1 but where it really 
shined was the precision of .09 for high-risk loans. This was nine times better than all models except for the Balanced Random Forest 
Classifier, where it was three times better. The highest recall values were also observed in this model where both high-risk and
low-risk loans were above .90 making the Easy Ensemble Classifier model the obvious winner. 