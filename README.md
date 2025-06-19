# Country-Risk-Investment

## Application of k-Means Clustering to Country Investment Risk

This analysis applies KMeans clustering to group countries based on key risk indicators. The goal is to identify clusters of countries that share similar risk profiles, which could be useful for investors, analysts, or policy professionals working with country-level risk assessments.

## Methods and Approach

We used the KMeans algorithm, a commonly used unsupervised machine learning technique, to segment the dataset into clusters. Before clustering, the data was cleaned and prepared to ensure all features were numeric—this is required by KMeans, which calculates distances between points.

To decide how many clusters to use, we evaluated clustering solutions for 2 to 10 clusters and calculated the silhouette score for each one. The silhouette score measures how well the countries fit within their assigned cluster, compared to others. Scores closer to 1 suggest well-separated and meaningful clusters.

## Results

Among the different options tested, the 3-cluster solution performed the best, with the highest average silhouette score (~0.353). This indicates that the countries in each group are reasonably distinct from one another. Other cluster numbers like 2, 8, and 9 also had decent scores, but none outperformed the 3-cluster model. The 5-cluster setup performed poorly, with a low silhouette score (~0.277), suggesting that it did not create clear groupings.

## Summary
	•	The data was clustered using KMeans after preprocessing.
	•	Silhouette scores helped determine the best number of clusters.
	•	The 3-cluster solution was the most effective, balancing interpretability and separation quality.

This clustering exercise offers a starting point for deeper analysis of country risk patterns, and the framework can be expanded with additional data or used to monitor changes over time.
