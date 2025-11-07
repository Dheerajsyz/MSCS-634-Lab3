# MSCS 634 Lab 3 - K-Means and K-Medoids Clustering

## Project Overview

This lab explores clustering techniques using K-Means and K-Medoids algorithms on the Wine Dataset from sklearn to analyze and compare clustering performance through visualizations and evaluation metrics.

## Dataset

- **Source**: sklearn.datasets.load_wine()
- **Classes**: 3 wine types
- **Features**: 13 chemical properties
- **Instances**: 178 samples
- **Preprocessing**: Z-score normalization (StandardScaler)

## Implementation

### K-Means Clustering
- Algorithm: K-Means with k=3
- Evaluation: Silhouette Score, Adjusted Rand Index

### K-Medoids Clustering
- Algorithm: K-Medoids with k=3
- Evaluation: Silhouette Score, Adjusted Rand Index

## Key Findings

### K-Means Results
- **Silhouette Score**: 0.2849
- **Adjusted Rand Index**: 0.8975
- Better cluster separation and definition
- Higher agreement with true wine classes

### K-Medoids Results
- **Silhouette Score**: 0.2676
- **Adjusted Rand Index**: 0.7411
- Slightly lower performance than K-Means
- More robust to outliers due to medoid-based centers

### Comparison Analysis
<img width="1590" height="590" alt="image" src="https://github.com/user-attachments/assets/dd59e48c-be1e-4d66-8506-b31caf4abd37" />

- **K-Means performed better** on this dataset with higher scores on both metrics
- K-Means achieved 89.75% agreement with true labels vs K-Medoids' 74.11%
- Both algorithms successfully identified 3 distinct clusters
- Visualization shows similar cluster patterns with different centroid/medoid positions
- K-Means centroids positioned at mean of clusters
- K-Medoids medoids are actual data points from the dataset

