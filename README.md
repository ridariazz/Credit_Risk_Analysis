# Overview

We employed different techniques to train and evaluate models with unbalanced classes as credit risk is an inherently unbalanced classification problem since good loans outnumber with unbalanced classes. Techniques we used are imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Moreover, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We will also compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once we're done with everything above, we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

# Results 

The results for the six machine learning models we used to describe the balanced accuracy scores and the precision are as follows: 

## 1. Naive Random Oversampling

![balance accuracy](https://user-images.githubusercontent.com/106577074/195959510-0e5b7f3c-2a13-402e-ba55-bf9511e13661.png)

![naive_random_oversampling2](https://user-images.githubusercontent.com/106577074/195959543-b58c5ea0-62ea-4d46-a26b-5c96449efb53.png)

*Balanced accuracy:* 0.6314677834584286

*Precision:* is low for high-risk loans (0.01) and high for low-risk loans (1.00)

*Recall:* 0.58/0.69

## 2. SMOTE Oversampling 

![smote_over](https://user-images.githubusercontent.com/106577074/195959584-b7996ddb-f495-4a7d-8fa9-b352b64185ff.png)

![smote_oveer2](https://user-images.githubusercontent.com/106577074/195959611-a3b94b59-148b-4ca9-ae9c-abdec0a37e58.png)

*Balanced accuracy:* 0.6268316069795457

*Precision:* is low for high-risk loans (0.01) and high for low-risk loans (1.00)

*Recall:*[- 0.61/0.64

## 3. SMOTE Undersampling

![under](https://user-images.githubusercontent.com/106577074/195959695-494de8ed-50c1-4646-a5bb-c8a0f289f528.png)

![under2](https://user-images.githubusercontent.com/106577074/195959702-9a07e111-3933-45b4-8dbb-e03d231e16ef.png)

*Balanced accuracy:* 0.6268316069795457

*Precision:* is low for high-risk loans (0.01) and high for low-risk loans (1.00)

*Recall:* 0.61/0.45

## 4. Combination 

![combo1](https://user-images.githubusercontent.com/106577074/195959727-be27a155-01da-4bd3-8ec7-8b6aec47d083.png)

![combo2](https://user-images.githubusercontent.com/106577074/195959735-fc4beb3a-924b-4a33-b587-199cbbb713df.png)

*Balanced accuracy:* 0.6413505042081133

*Precision:* is low for high-risk loans (0.01) and high for low-risk loans (1.00)

*Recall:* 0.70/0.58

## 5. Balanced Random Forest Classifier

![balance accuracy3](https://user-images.githubusercontent.com/106577074/195959749-a28a2735-52a1-47a8-8950-293b4fc79963.png)

![recall](https://user-images.githubusercontent.com/106577074/195959753-1fa08610-04b4-44b0-a9ad-982b1778eea3.png)

*Balanced accuracy:* 0.7877672625306695

*Precision:* is low for high-risk loans (0.04) and high for low-risk loans (1.00)

*Recall:* 0.67/0.91

## 6. Easy Ensemble AdaBoost Classifier

![Screen Shot 2022-10-14 at 4 57 22 PM](https://user-images.githubusercontent.com/106577074/195959785-c28e0210-1f91-4c35-9b01-5296d8e614f8.png)

![Screen Shot 2022-10-14 at 4 57 26 PM](https://user-images.githubusercontent.com/106577074/195959795-bd770e15-9358-46de-b8c9-57f1ed4246e1.png)

*Balanced accuracy:* 0.925427358175101

*Precision:* is low for high-risk loans (0.07) and high for low-risk loans (1.00)

*Recall:* 0.91/0.94

# Summary

The best model to use is the Easy Ensemble AdaBoost Classifier as it produced the highest accuracy score with 0.93 and had the higest recall score with the numbers closest to 1.0. The others models were below the 0.80 accuracy mark, so they are not the most accurate for data depiction of our analysis. 
