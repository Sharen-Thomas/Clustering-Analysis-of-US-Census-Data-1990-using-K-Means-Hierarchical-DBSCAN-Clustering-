# Clustering-Analysis-of-US-Census-Data-1990-using-K-Means-Hierarchical-DBSCAN-Clustering-

## OVERVIEW

This project performs unsupervised clustering analysis on the US Census Data 1990 dataset. Using three different clustering algorithms: K-Means, Hierarchical Clustering, and DBSCAN, we identify patterns, anomalies, and natural groupings within the population data. The analysis includes data preprocessing, standardization, dimensionality reduction via PCA, and comprehensive visualization of clustering results.

## WHAT IT DOES

### DATA PREPROCESSING
- Load 30,000 sample rows, check for null values, inspect categorical features

### STANDARDIZATION
- Scale features to ensure equal contribution to clustering

### DIMENSIONALITY REDUCTION 
- PCA to reduce features to 2 principal components for visualization

### K-MEANS CLUSTERING
- Elbow method + Silhouette score to determine optimal k=4

### HIERARCHICAL CLUSTERING
- Dendrogram analysis + Ward's linkage method

### DBSCAN CLUSTERING 
- K-distance graph to determine eps=3.0, MinPts=5

## KEY RESULTS

### OPTIMAL CLUSTERS BY ALGORITHM 

#### K-MEANS
- Optimal Clusters: 4
- Key Insight: Well-separated, spherical clusters

#### HIERARCHICAL 
- Optimal Clusters: 3
- Key Insight: Nested structure with macro-level groupings

#### DBSCAN 
- Optimal Clusters: 130+
- Key Insight: Many small dense regions + outliers detected

### CLUSTER QUALITY ASSESSMENT 

#### K-MEANS
- Quality: Excellent
- Strengths: High separation, high cohesion
- Weaknesses: Requires k beforehand, sensitive to outliers

#### HIERARCHICAL 
- Quality: Good
- Strengths: Detects nested patterns, flexible
- Weaknesses: Vulnerable to noisy data

#### DBSCAN
- Quality: Excellent
- Strengths: Identifies outliers, irregular shapes
- Weaknesses: Parameter sensitive

### VISUAL PATTERNS DISCOVERED 

- **K-Means (k=4)**: Blue cluster distinctly isolated; green/orange clusters overlap; pink cluster sparse (potential outliers)
- **Hierarchical (k=3**): Red cluster highly separate; blue/green clusters show partial overlap
- **DBSCAN**: 130+ micro-clusters detected; significant noise points (label = -1); non-spherical shapes captured

## TECH STACK 

- Language: Python
- Data Processing: Pandas, NumPy
- Preprocessing: Scikit-learn (StandardScaler)
- Dimensionality Reduction: PCA (Principal Component Analysis)
- Clustering: KMeans, AgglomerativeClustering, DBSCAN
- Evaluation: Elbow Method, Silhouette Score, K-Distance Graph
- Visualization: Matplotlib, Seaborn

## KEY GRAPHS GENERATED 

- Elbow Curve: Determine optimal k for K-Means
- Silhouette Score: Validate cluster separation quality
- Dendrogram:	Visualize hierarchical clustering structure
- K-Distance Graph:	Determine eps parameter for DBSCAN
- PCA Scatter Plots:	Visualize clusters in 2D space

## FILES 

- 'INFO411_Project_Report.pdf' - Complete project documentation

## DISCLAIMER
**This repository is for viewing purposes only. It is not licensed for copying, modification, or commercial use without explicit permission from the author.**
