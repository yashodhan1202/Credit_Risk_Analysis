# Credit_Risk_Analysis

# Analysis Overview

In this project, we had to use Python to build and evaluate several machine learning models to predict credit risk. We adopted the following procedure:

1) Oversample the data using the RandomOverSampler and SMOTE alogrithms
2) Undersample the data using the ClusterCentroids algorithm
3) Combinational approach of over and undersampling using SMOTEENN alogrithm 
4) Compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier 

We had to evaluate the performance of these models and make a recommendation on whether they should be used to predict credit risk

# Results

**Naive Random Oversampling results (Using the RandomOverSampler algorithm)** :- The balanced accruacy test is 66%, the precision for the high-risk is 1% with a sensitivity of 74%. The precision for low-risk is 100% with a sensitivity of 58%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/Naive_Random_Oversampling.png)

**Oversampling results (Using SMOTE algorithm):** The balanced accruacy test is 65.3%, the precision for the high-risk is 1% with a sensitivity of 62%. The precision for low-risk is 100% with a sensitivity of 68%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/SMOTE_Oversampling.png)

**Undersampling results (Using ClusterCentroids Algorithm)**: The balanced accruacy test is 65.3%, the precision for the high-risk is 1% with a sensitivity of 69%. The precision for low-risk is 100% with a sensitivity of 40%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/Cluster_Centroids_Undersampling.png)

**Combination(over and undersampling) results (Using SMOTEENN algorithm):** The balanced accruacy test is 54.4%, the precision for the high-risk is 1% with a sensitivity of 72%. The precision for low-risk is 100% with a sensitivity of 57%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/SMOTEENN_Combo.png)

**Balanced Random Forest Classifier results:** The balanced accruacy test is 76.5%, the precision for the high-risk is 3% with a sensitivity of 65%. The precision for low-risk is 100% with a sensitivity of 88%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/Balanced_Random_Forest_Classifier.png)

**Easy Ensemble AdaBoost Classifier results:** The balanced accruacy test is 91.7%, the precision for the high-risk is 9% with a sensitivity of 89%. The precision for low-risk is 100% with a sensitivity of 94%.

![Image](https://github.com/yashodhan1202/Credit_Risk_Analysis/blob/main/Easy_Ensemble_AdaBoost_Classifier.png)

# Summary

All the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high.The Ensemble models brought a lot more improvment specially on the sensitivity of the high risk credits.The EasyEnsembleClassifier model shows a recall of 91.7% so it detects almost all high risk credit. On another hand, with a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities.Typically in your models you want a good balance of recall and precision. For these reasons I would not recommend the bank to use any of these models to predict credit risk.
