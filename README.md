# Clustering Algorithm
## Objective
The objective of this assessment is to evaluate the ability to apply clustering techniques to a real-world dataset, using the Iris dataset from sklearn. The goal is to implement KMeans and Hierarchical clustering algorithms, and visualize their results.

## Dataset
The dataset used in this project is the Iris dataset. It contains measurements of 150 iris flowers across 4 features:

(1) Sepal length
(2) Sepal width
(3) Petal length
(4) Petal width

Steps 
1. Loading and Preprocessing
The Iris dataset is loaded using sklearn.datasets.load_iris() and preprocess the data by removing the duplicates

2. Clustering Algorithm Implementation
A) KMeans Clustering
Description: KMeans clustering is an iterative algorithm that divides data points into a predefined number of clusters, k. It works by:
Initializing k centroids randomly.
Assigning each data point to the nearest centroid.
Updating the centroids by calculating the mean of the points in each cluster.
Repeating the above steps until convergence.
The Iris dataset is relatively simple and well-suited for KMeans as it has clear groupings of data points based on the flower species.
KMeans works well when the clusters are spherical and roughly equal in size, which is a good assumption for the Iris dataset.

B) Hierarchical Clustering
Description: Hierarchical clustering builds a tree of clusters, also known as a dendrogram. It works in two main ways:

Agglomerative (bottom-up): Starts with each data point as its own cluster and merges the closest clusters iteratively.
Divisive (top-down): Starts with all data points in one cluster and splits the clusters iteratively.
Hierarchical clustering does not require a predefined number of clusters.
It works well for smaller datasets like the Iris dataset and is helpful in visualizing the hierarchy of clusters.

## Conclusion
Both clustering algorithms, KMeans and Hierarchical clustering, were successfully applied to the Iris dataset. The KMeans algorithm divided the dataset into 3 clusters, which matched the known species of the flowers. Hierarchical clustering also provided a similar result, but with a different approach to determining the clusters.

The choice of algorithm depends on the dataset characteristics and the need for interpretability:

KMeans is faster and more efficient for large datasets but requires specifying the number of clusters beforehand.
Hierarchical clustering provides a more detailed clustering structure and does not require the number of clusters to be predefined.
