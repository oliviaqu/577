# Ensemble Method

## Introduction

Ensemble methods are machine learning methods that aggregate the predictions of a group of base learners in order to form a single learning model.

Ensemble methods involve aggregating multiple machine learning models with the aim of decreasing both bias and variance. 
Ideally, the result from an ensemble method will be better than any of individual machine learning model.

There are 3 main types of ensemble methods:

#### - Bagging

#### - Boosting

#### - Stacking

In this folder, we only focus on bagging. We examine machine learning model: **Random Forest** which utilises the technique of bagging.

## Random forest (bagging)

### Introduction

Bagging, also known as bootstrap aggregating, refers to the process of creating and merging a collection of **independent, parallel** decision trees using different subsets of the training data (bootstrapped datasets).

### Illustration

<img src="https://user-images.githubusercontent.com/98184249/163267120-b4199e55-19db-41c7-9bf6-2143e5081385.svg" width="500px">
<img src="https://user-images.githubusercontent.com/98184249/163267466-20c445f3-90dc-49d1-8a87-9a301d169be2.png" width="500px">


### Feature

Decision trees built using random forest have zero knowledge and influence on the other trees in the model. This is a key defining feature of bagging.

it is clear that bagging reduces the dependence on a single tree by spreading the risk of error across multiple trees, which also indirectly reduces 
the risk of overfitting.

To wrap up on random forest, here are some key hyperparameters to consider:

**n_estimators:** controls how many individual decision trees will be built

**max_depth:** controls how deep each individual decision tree can go


### Advantages V.S Disadvantages

### Advantages(When to use random forest)

It can be used for both classification (RandomForestClassifier)and regression (RandomForestRegressor) problems

You are interested in the significance of predictors (feature importance)

You need a quick benchmark model as random forest are quick to train and require minimal preprocessing e.g. feature scaling

If you have messy data e.g. missing data, outliers etc

### Disadvantages(When not to use random forest)

If you are solving a complex, novel problem

Transparency is important

Prediction time is important as the model needs time to aggregate the result from multiple decision trees before arriving at the final prediction


# DATASET

The dataset used is palmerpenguins which contains size measurements for three penguin species observed on three islands in the Palmer Archipelago, Antarctica.

In this Ensembel method, we first use 'bill length[mm]' and 'bill depth[mm]' as features to train the bagging and random forest model and make the comparision through classification report.

Then, we consider all features in penguin dataset and compare decision tree model, bagging model and random forest model through classification report and decision boundary plots.
