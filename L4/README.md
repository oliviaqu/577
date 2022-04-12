# Nonparametric modeling: The K-Nearest Neighbors Algorithm

## Definition

The 𝑘-nearest neighbors algorithm, or KNN for short, is a nonparametric algorithm that assumes that similar data exist in close proximity. In other words, similar things are near to each other.

KNN captures the idea of similarity (sometimes called distance, proximity, or closeness) with some mathematics we might have learned in our childhood— calculating the distance between points on a graph.

KNN is a non-parametric supervised model, and its main idea is to classify or regress by compute the k closest training examples in the data set.

## KNN Algorthm

Take a look at the two-dimension space, we can have a intuitive idea about how knn works. The following figure by Navlani (link) clearly illustrates the algorithm of KNN.

Given the samples and the new data point in the sample space, distances between the new example data point and all other points are calculated and ranked ascending. Then the first k samples are picked up, and a majority vote (for classification) or an average (for regression) is taken among the top k samples to predict label of the new example.

![knn_illu](https://user-images.githubusercontent.com/98184249/162826229-66f5ce3d-dcaa-44f0-a3bc-cabfc282daf7.png)

## Advantages V.S Disadvantages
### Advantages
The algorithm is simple and easy to implement.

There’s no need to build a model, tune several parameters, or make additional assumptions.

The algorithm is versatile. It can be used for classification, regression, and search (as we will see in the next section).

### Disadvantages

The algorithm gets significantly slower as the number of examples and/or predictors/independent variables increase.

# DATASET

### Classification

The dataset used is palmerpenguins which contains size measurements for three penguin species observed on three islands in the Palmer Archipelago, Antarctica.

In this KNN alogrithm, we use 'bill length[mm]' and 'bill depth[mm]' as features to train the model and make the classification.

### Regression

The dataset used is California housing dataset, we try to use KNN to solve regression problem. But, the result does not seem to be satisfactory, which shows faced with multiply variables, the KNN seems to be unsuitable.
