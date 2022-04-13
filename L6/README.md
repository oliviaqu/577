# Decision Tree and Regression Tree

## Introduction

Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features. A tree can be seen as a piecewise constant approximation.

## Decision Tree Alogrithm

Decision trees tend to be the method of choice for predictive modeling because they are relatively easy to understand and are also very effective. The basic goal of a decision tree is to split a population of data into smaller segments. There are two stages to prediction. The first stage is training the model—this is where the tree is built, tested, and optimized by using an existing collection of data. In the second stage, you actually use the model to predict an unknown outcome.

Decision trees are constructed from only two elements — nodes and branches.
<img src='https://user-images.githubusercontent.com/98184249/163085650-bc1cba73-095d-403c-9099-3ffde717a68f.jpeg' width='500px'>

The nodes shown above fall under the following types of nodes:

#### Root node — node at the top of the tree. This node acts as the input node for feature vectors in the model.
#### Decision nodes — nodes where the variables are evaluated. These nodes have arrows pointing to them and away from them
#### Leaf nodes — final nodes at which the prediction is made

## Advantages V.S Disadvantages

### Advantages
Easy to use and understand.

Can handle both categorical and numerical data.

Resistant to outliers, hence require little data preprocessing.

### Disadvantages

Disadvantage of Decision Tree

Prone to overfitting

Require some kind of measurement as to how well they are doing

Need to be careful with parameter tuning

Can create biased learned trees if some classes dominate.

# DATASET
