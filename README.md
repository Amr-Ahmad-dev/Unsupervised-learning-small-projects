# 🌌 Unsupervised Clustering: K-Means & DBSCAN

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-F7931E.svg)](https://scikit-learn.org/)
[![Topic](https://img.shields.io/badge/Topic-Unsupervised%20Clustering-darkblue.svg)](#)

## 📌 Project Overview
This project presents an empirical comparison between two widely used clustering paradigms: K-Means (centroid-based) and DBSCAN (density-based), demonstrating how each algorithm segments synthetic multi-cluster datasets and handles anomalies.

---

## 🔬 Algorithms Compared
```
                    Unsupervised Clustering
                               │
               ┌───────────────┴───────────────┐
               ▼                               ▼
       [K-Means Clustering]           [DBSCAN Clustering]
      Centroid-based Partition       Density-connected Topology
      Predefined cluster count $k$   Finds arbitrary shapes
      Forces every point into $k$    Labels outliers as noise (-1)
```

### 1. K-Means
- Fits spherical clusters around $k=3$ initialized centroids.
- Visualizes cluster assignment maps and plots converged cluster centers marked with red `'X'`.

### 2. DBSCAN
- Parameterized with `eps=0.3` and `min_samples=5`.
- Identifies continuous density regions regardless of cluster geometry.
- Flags non-reachable points as noise ($y = -1$) and highlights them visually with prominent red outlier markers.

---

## 💻 Code Structure
- **Notebook**: [`unsupervised_clustering_kmeans_dbscan.ipynb`](./unsupervised_clustering_kmeans_dbscan.ipynb)
- **Cell Count**: 16 cells (14 code cells, 2 markdown cells)
- **Dependencies**: `scikit-learn`, `numpy`, `matplotlib`

---

## 🚀 How to Run
```bash
pip install scikit-learn numpy matplotlib
jupyter notebook unsupervised_clustering_kmeans_dbscan.ipynb
```
