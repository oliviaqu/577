# K_Means Clustering

## Definition

K-Means Clustering is a method of vector quantization, originally from signal processing, that aims to partition n observations into k clusters in which each observation belongs to the cluster with the nearest mean (cluster centers or cluster centroid), serving as a prototype of the cluster. This results in a partitioning of the data space into Voronoi cells.

<img src="https://user-images.githubusercontent.com/98184249/163904130-31156d09-d6c2-40f8-9acc-31bf45ebed28.png" width="600px">


## Advantages V.S Disadvantages

### Advantages
- Relatively simple to implement.
- Scales to large data sets.
- Guarantees convergence.
- Can warm-start the positions of centroids.
- Easily adapts to new examples.
- Generalizes to clusters of different shapes and sizes, such as elliptical clusters.

### Disadvantages
- Choosing k manually.
- Being dependent on initial values.

-- For a low K, you can mitigate this dependence by running k-means several times with different initial values and picking the best result. As K increases, you need advanced versions of k-means to pick better values of the initial centroids (called k-means seeding).
- Clustering data of varying sizes and density.

--  k-means has trouble clustering data where clusters are of varying sizes and density. To cluster such data, you need to generalize k-means as described in the Advantages section.
- Clustering outliers.

-- Centroids can be dragged by outliers, or outliers might get their own cluster instead of being ignored. Consider removing or clipping outliers before clustering.
- Scaling with number of dimensions.
As the number of dimensions increases, a distance-based similarity measure converges to a constant value between any given examples.

# DATASET
The dataset used is palmerpenguins which contains size measurements for three penguin species observed on three islands in the Palmer Archipelago, Antarctica.

In this KNN alogrithm, we use 'bill length[mm]' and 'bill depth[mm]' as features to train the model and make the classification.

We first build the class about k-means clustering from the scratch, then perform the algorithm again using scikit-learn package.
