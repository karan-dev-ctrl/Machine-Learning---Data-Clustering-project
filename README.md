📊 Google Review Ratings – Clustering Analysis

Unsupervised Machine Learning Project using K-Means, DBSCAN, and Spectral Clustering

📌 Project Overview

This project performs clustering analysis on the Google Review Ratings dataset to discover natural user behavior patterns across 24 rating categories (restaurants, parks, beaches, museums, hotels, etc.).
Three clustering algorithms were evaluated:

1. K-Means Clustering

2. DBSCAN (Best Performing Model)

3. Spectral Clustering

All models were evaluated using silhouette scores and visualized using PCA (2D).

📁 Dataset

5456 user records

24 average review rating features

Rating values range from 0 to 5

Dataset includes categories like:

Restaurants, Cafes, Pubs/Bars

Parks, Beaches, Zoos

Museums, Art Galleries, Monuments

Hotels, Resorts, Local Services

And many more...

🛠 Technologies & Libraries:

Python

Scikit-Learn

Pandas, NumPy

Matplotlib

PCA (Dimensionality Reduction)

K-Means, DBSCAN, Spectral Clustering

StandardScaler

🔧 Preprocessing Steps

✔ Removed irrelevant columns
✔ Converted all values to numeric
✔ Handled missing values with median imputation
✔ Standardized data using StandardScaler
✔ Reduced dimensionality for visualization using PCA (2D)

🚀 Clustering Experiments:

1️⃣ K-Means Clustering:

Optimal k = 3 determined using Elbow Method

Silhouette Score: 0.145

Formed 3 broad clusters but with overlap

2️⃣ DBSCAN (Best Model):

Parameters: eps = 0.7, min_samples = 5

Silhouette Score: 0.669 (highest)

Detected meaningful high-density clusters

Successfully isolated noise/outlier points

3️⃣ Spectral Clustering:

Used n_clusters = 3

Silhouette Score: 0.099

Detected non-linear structure but weak separation

📷 Visualizations Included

PCA scatter plots for:

K-Means (3 clusters)

DBSCAN (cluster + noise)

Spectral Clustering (3 clusters)

Elbow method plot

🏁 Conclusion

DBSCAN proved to be the most effective clustering algorithm for the Google Review Ratings dataset, producing the strongest cluster separation and the highest silhouette score (0.669).
It successfully captured natural density-based user rating patterns that K-Means and Spectral Clustering could not.
