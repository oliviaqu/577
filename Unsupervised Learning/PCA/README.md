# Principal Component Analysis (PCA)

## Definition

**Principal Component Analysis (PCA)** is used in exploratory data analysis and for multidimensionality reduction. The main idea is to project data points onto only the first few principal components to obtain lower-dimensional data while preserving as much of the data’s variation as possible. In other words, using PCA we remove the redundant and highly-correlated data and we keep only the most significant data features for further analysis.


<img src="https://user-images.githubusercontent.com/98184249/164307379-e9d18c69-b74d-435b-af37-05272214a8bf.png" width="500px">

The goal of PCA is to reduce the dimensionality of the feature vectors used in training machine learning algorithms.

# DATASET
The dataset used is palmerpenguins which contains size measurements for three penguin species observed on three islands in the Palmer Archipelago, Antarctica.

Since the result of K-means clustering just using 'bill length' and 'bill depth' these two features is not satisfactory, this time
we still use the penguin dataset, but all the penguins features are considered. We first use the PCA to reduce the dimension and use the kmeans clustering to
cluster the penguin species.
