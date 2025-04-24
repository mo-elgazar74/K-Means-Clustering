# K-Means Clustering with PCA: 2D & 3D Visualization + Elbow Method

This project demonstrates **K-Means Clustering** using Python, featuring PCA-based dimensionality reduction for 2D and 3D cluster visualization, alongside the elbow method for optimal cluster selection, and interactive plotting. It’s ideal for understanding the fundamentals of unsupervised learning and how PCA can improve visualization of high-dimensional data.

## 📊 Dataset

We use the [Facebook Live Sellers in Thailand dataset](https://www.kaggle.com/datasets/ashishg21/facebook-live-sellers-in-thailand-uci-ml-repo) from Kaggle, originally published by the UCI ML Repository. It contains features related to live commerce sessions such as likes, comments, shares, product category, and more.

Download the dataset from Kaggle and place the file in the same directory as the notebook.

## 📁 Files

- `k-means-clustering.ipynb`: Jupyter notebook implementing clustering, PCA, visualizations, and evaluation.
- `README.md`: This file.

## 📦 Libraries Used

- `pandas` — for dataset manipulation
- `numpy` — for numerical operations
- `matplotlib` — for 2D and 3D plotting
- `seaborn` — for enhanced visual styling
- `scikit-learn` — for `KMeans`, `PCA`, and preprocessing
- `kneed` — to find the optimal number of clusters using the elbow method

## 🧪 Workflow

### 1. 📊 Data Loading
Load and inspect the dataset before analysis.

### 2. ⚙️ Preprocessing
Data is cleaned and scaled using `StandardScaler` to improve clustering performance.

### 3. 📉 Elbow Method (with `kneed`)
The elbow method determines the optimal number of clusters.
We plot the Within-Cluster Sum of Squares (inertia) vs. `k` and use `KneeLocator` to automatically detect the elbow point.

### 4. 🚀 Clustering
K-Means is applied with the selected number of clusters.

### 5. 🔄 Dimensionality Reduction (PCA)
PCA is applied to project the high-dimensional data into:
- **2D** for standard scatter visualization
- **3D** for a spatial perspective of cluster separation

### 6. 📊 Visualization
- **2D Scatter plot** with colored clusters and centroids.
- **3D Scatter plot** for multi-dimensional visualization of cluster separation.
- **Elbow curve** for cluster evaluation

## ▶️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/k-means-clustering.git
   cd k-means-clustering
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn kneed
   ```

3. Run the notebook:
   ```bash
   jupyter notebook k-means-clustering.ipynb
   ```

## 🔍 Example Output

- Clear 2D and 3D PCA projections of clusters
- Elbow curve showing the optimal number of clusters
- Visually distinct cluster separation in reduced dimensions

## 🛠️ Future Enhancements

- Allow dynamic dataset uploads (e.g., upload CSV)
- Integrate clustering metrics comparison (e.g., DBSCAN, Agglomerative)

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
