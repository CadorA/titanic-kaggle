# Titanic - Machine Learning from Disaster - Top 7%

This repository contains the notebook which I used to attend the related Kaggle competition. The objective is to predict the number of the survivors.

## Structure
The notebook starts with a short description of the problem.

Afterwards, the Exploratory Data Analysis begins, looking at the given features, plotting useful figures and comparing the value counts for different combinations of features (such as Roadtype-Crime Category).

The models I used are presented below:
1. SVM - Good baseline accuracy.
2. Random Forrest - Used to obtain the best test accuracy (0.79)
3. LightGBM - Fast to train Gradient Boosting
4. CatBoost and XGBoost - Used to benchmark other version. Unfortunately, the training time is big and the accuracy is much similar to LGB.
5. K-Nearest Neighbours (KNN) Classifier - Simple and good for initial insights.
6. StackingClassifier - I stacked the results from (SVM, RF, LGBM, KNN) using a Logistic Regression as the final layer.

For the tuning of the previous models, I used both RandomSearchCV,GridSearchCV (from sklearn) and Optuna.

## Results
The best result was obtained using RandomForestClassifier() -  Top 7%

**A detailed article that contains the insights and the explanations of the strategy used can be found on my Medium page: [Link Medium Page - To be updated]**
