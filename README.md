# Project Overview
Fast Lending uses machine learning to predict credit risk for quicker, more reliable data to determine good loan candidates. This in turn helps reduce their loan default rate. Credit risk is an inherently unbalanced classification of machine learning because good loans easily outnumber risky loans. Therefore, different machine learning techniques are needed to train and evaluate modles with unbalanced classes. Using imbalanced-learn and scikit-learn libraries, various machine learning models will be used to build a model for Fast Lending to use to predict good loan candidates.

# Class Imbalance
Class imbalance refers to a situation in which exising classes are unequally represented. This imbalance causes machine learning models to be biased towards the majority class in a dataset. The goal of machine learning models for Fast Lending is to identify where the minority class of risky loans exists. Three ways to overcome this imbalance is with random oversampling, synthetic minority oversampling techiques (SMOTE) and random undersampling.

## Random Oversampling
Random oversampling uses the minority class and randomly selects data to add to the training set until the majority and minority classes are balanced.
![image](https://user-images.githubusercontent.com/99636479/174398630-27f3ef90-a9e5-40a4-ba6a-196167fc865d.png)


## SMOTE
SMOTE is similar to random oversampling where the size of the minority class is increased to be balanced with the majority class. The key difference is SMOTE creates new instances of data based on the values of neighboring values.
![image](https://user-images.githubusercontent.com/99636479/174398567-d5e98e4d-8cf1-4af9-bac7-0420ee263543.png)

## Random Undersampling
randomly selected instances from the majority class are removed until the size of the majority class is reduced, typically to that of the minority class. The dataset used in this example contains information on credit card default.
