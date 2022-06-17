# Project Overview
Fast Lending uses machine learning to predict credit risk for quicker, more reliable data to determine good loan candidates. This in turn helps reduce their loan default rate. Credit risk is an inherently unbalanced classification of machine learning because good loans easily outnumber risky loans. Therefore, different machine learning techniques are needed to train and evaluate modles with unbalanced classes. Using imbalanced-learn and scikit-learn libraries, various machine learning models will be used to build a model for Fast Lending to use to predict good loan candidates.

# Class Imbalance
Class imbalance refers to a situation in which exising classes are unequally represented. This imbalance causes machine learning models to be biased towards the majority class in a dataset. The goal of machine learning models for Fast Lending is to identify where the minority class of risky loans exists. Four ways to overcome this imbalance is with random oversampling, synthetic minority oversampling techiques (SMOTE), random undersampling, and combination of SMOTE and Edited Nearest Neighbors (SMOTEENN).

### *Random Oversampling
Random oversampling uses the minority class and randomly selects data to add to the training set until the majority and minority classes are balanced.
![image](https://user-images.githubusercontent.com/99636479/174398630-27f3ef90-a9e5-40a4-ba6a-196167fc865d.png)


### *SMOTE
SMOTE is similar to random oversampling where the size of the minority class is increased to be balanced with the majority class. The key difference is SMOTE creates new instances of data based on the values of neighboring values.
![image](https://user-images.githubusercontent.com/99636479/174398567-d5e98e4d-8cf1-4af9-bac7-0420ee263543.png)

### *Random Undersampling
Random undersampling removes randomly selected instances of the majority class to balance with the minority class. 
![image](https://user-images.githubusercontent.com/99636479/174400969-3adb38d7-35a8-4ee5-baa7-ca354d6df5cb.png)

### *SMOTEENN
SMOTEENN oversample the minority class with SMOTE and then cleans the resulting data with an undersampling strategy. If the two nearest neighbors of a data point belong to two different classes, that data point is dropped.
![image](https://user-images.githubusercontent.com/99636479/174402324-5a55a64d-5ca5-4ba2-af9d-8fd765c08253.png)

# Ensemble Learning
Ensemble learning is the process of combining multiple models, like decision tree algorithms, to help improve the accuracy and robustness and decrease variance of the model. This results in an increase in the overall performance of the model. Two examples of ensemble learning is balanced random forest classifier and easy ensemble adaBoost classifier.

A balanced random forest randomly under-samples each boostrap sample to balance it.

### *Balanced Random Forest Classifier
Balanced random forest classifier randomly under-samples each boostrap sample to balance it. Bootstrapping is a sampling technique that randomly selects samples and returns back to the general pool.
![image](https://user-images.githubusercontent.com/99636479/174406682-bccdc3d6-c768-4b42-bbda-7c429ad5fef5.png)


### *Easy Ensemble AdaBoost Classifier
Easy ensemble adaBoost classifier (i.e. BalancedBaggingClassifier) takes each bootstrap sample to be further resampled to achieve sampling strategy desired. 
![image](https://user-images.githubusercontent.com/99636479/174406471-0e2945df-3e65-45d0-815a-f5a0a5214fe3.png)


# Summary

