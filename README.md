<h1 align="center">🧩 Clustering Playground 🧩</h1>
<h3 align="center">Exploring Unsupervised Learning — One Algorithm at a Time</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikit-learn" />
  <img src="https://img.shields.io/badge/Unsupervised-Learning-purple?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge" />
</p>

---

## 📌 What is this repo?

Clustering is one of the most fundamental ideas in unsupervised machine learning — grouping data points based on similarity without any labeled guidance.

This repo is my personal playground for exploring different clustering algorithms hands-on. Each notebook covers one algorithm from scratch — the theory, the implementation, the visualization, and the evaluation. No shortcuts, just genuine understanding.

> Currently adding algorithms one by one. Stay tuned. 🚀

---

## 📁 Repository Structure

```
Clustering-Playground/
├── kmeans/
│   ├── images/
│   │   ├── elbow_curve.png
│   │   ├── silhouette_plot.png
│   │   └── kmeans_clusters.png
│   └── kmeans_clustering.ipynb
│
├── dbscan/                     # Coming soon
├── hierarchical/               # Coming soon
└── README.md
```

---

## 🗂️ Algorithms Covered

| # | Algorithm | Notebook | Status |
|---|-----------|----------|--------|
| 1 | K-Means Clustering | `kmeans/kmeans_clustering.ipynb` | ✅ Done |
| 2 | DBSCAN | `dbscan/` | 🔜 Coming Soon |
| 3 | Hierarchical / Agglomerative | `hierarchical/` | 🔜 Coming Soon |

---

## 🔵 1. K-Means Clustering

**File:** `kmeans/kmeans_clustering.ipynb`

K-Means partitions data into K groups by minimizing within-cluster variance. It's simple, fast, and a great starting point for clustering.

### Workflow
1. Generate synthetic data using `make_blobs` (1000 samples, 3 centers)
2. Standardize features using `StandardScaler`
3. Run the **Elbow Method** to find the optimal K value
4. Validate K using the **Silhouette Score**
5. Auto-detect the elbow point using `KneeLocator`
6. Fit final model with `k=3` and visualize clusters

### Key Concepts Applied
- `init="k-means++"` — smarter centroid initialization vs random
- WCSS (Within-Cluster Sum of Squares) as the inertia metric
- Silhouette Coefficient for quantitative cluster quality
- Proper scaling before clustering (scale-sensitive algorithm)

### Results

<p align="center">
  <img src="kmeans/images/elbow_curve.png" alt="Elbow Curve" width="45%"/>
  &nbsp;&nbsp;
  <img src="kmeans/images/silhouette_plot.png" alt="Silhouette Score" width="45%"/>
</p>

<p align="center">
  <img src="kmeans/images/kmeans_clusters.png" alt="K-Means Clusters" width="60%"/>
</p>

---

## 🛠️ Libraries Used

- `scikit-learn`
- `numpy`
- `matplotlib`
- `kneed`

---

## 🚀 How to Run

**1. Clone the repo**
```bash
git clone https://github.com/AnmolPatel20/Clustering-Playground.git
cd Clustering-Playground
```

**2. Install dependencies**
```bash
pip install numpy matplotlib scikit-learn kneed
```

**3. Open any notebook**
```bash
jupyter notebook kmeans/kmeans_clustering.ipynb
```

---

## 📌 Notes

- All notebooks use synthetic datasets (no downloads needed)
- Always scale features before clustering — most algorithms are distance-based and scale-sensitive
- Each algorithm folder is self-contained with its own images

---

## 🙋 About

I'm on my machine learning journey — building, experimenting and documenting as I go. Every notebook here represents something I've genuinely tried to understand, not just run. 🚀

- GitHub: [@AnmolPatel20](https://github.com/AnmolPatel20)
- Portfolio: [anmolpatel20.github.io/Anmol_Portfolio](https://anmolpatel20.github.io/Anmol_Portfolio/)

## 🙏 Acknowledgements

Thanks to **Krish Naik Sir** whose Udemy course has been a great resource throughout this learning journey.

*"Without data, you're just another person with an opinion." — W. Edwards Deming*

---

<p align="center">⭐ Star this repo if you found it helpful!</p>
