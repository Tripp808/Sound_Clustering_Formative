# Clustering Unlabeled Sound Data

## Overview
This project clusters unlabeled sound data using Mel Spectrogram features, dimensionality reduction (PCA, t-SNE), and clustering algorithms (K-Means, DBSCAN). The goal is to identify meaningful clusters and evaluate performance.

## Key Steps
1. **Feature Extraction:** Extract Mel Spectrogram features using Librosa.
2. **Dimensionality Reduction:** Apply PCA and t-SNE for visualization and clustering.
3. **Clustering:** Use K-Means (optimal `k` from Elbow Method) and DBSCAN.
4. **Evaluation:** Compare clustering performance using Silhouette Score and Davies-Bouldin Index.

## Results
- **K-Means:** Silhouette Score = 0.7005, Davies-Bouldin Index = 1.0313 (good separation).
- **DBSCAN:** Silhouette Score = -0.0305, Davies-Bouldin Index = 1.8554 (poor performance).
- **Visualization:** t-SNE provided better cluster separability than PCA.

## Challenges
- High dimensionality and overlapping data points made clustering difficult.
- DBSCAN struggled due to varying densities and parameter sensitivity.

## Conclusion
Dimensionality reduction (PCA, t-SNE) improved interpretability and clustering efficiency. K-Means performed well, while DBSCAN was less effective.
