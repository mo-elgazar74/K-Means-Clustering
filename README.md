# K-Means Clustering: 2D & 3D Visualization with the Elbow Method

This project demonstrates **K-Means Clustering** using Python, complete with 2D and 3D visualizations, elbow method analysis (via the `kneed` library), and interactive plotting. It’s ideal for understanding the fundamentals of unsupervised learning on real-world data.

## 📊 Dataset

We use the [Facebook Live Sellers in Thailand dataset](https://www.kaggle.com/datasets/ashishg21/facebook-live-sellers-in-thailand-uci-ml-repo) from Kaggle, originally published by the UCI ML Repository. It contains features related to live commerce sessions such as likes, comments, shares, product category, and more.

Download the dataset from Kaggle and place the file in the same directory as the notebook.

## 📁 Files

- `k-means-clustering.ipynb`: Jupyter notebook implementing the clustering algorithm, visualizations, and evaluation.
- `README.md`: This file.

## 📦 Libraries Used

- `pandas` — for dataset manipulation
- `numpy` — for numerical operations
- `matplotlib` — for 2D and 3D plotting
- `seaborn` — for enhanced visual styling
- `scikit-learn` — for `KMeans`, `make_blobs`, and preprocessing
- `kneed` — to find the optimal number of clusters using the elbow method

## 🧪 Workflow

### 1. 📊 Data Loading
The dataset is loaded and briefly explored for preprocessing and clustering.

### 2. ⚙️ Preprocessing
Data is cleaned and scaled using `StandardScaler` to improve clustering performance.

### 3. 📈 Elbow Method (with `kneed`)
The elbow method is used to find the optimal number of clusters. We plot the Within-Cluster Sum of Squares (inertia) vs. `k` and use `KneeLocator` to automatically detect the elbow point.

### 4. 🚀 Clustering
K-Means is applied with the optimal `k` and results are visualized in:
- 2D (scatter plots with cluster colors and centroids)
- 3D (using `Axes3D` from `matplotlib`)

### 5. 📉 Evaluation
While K-Means is unsupervised, inertia (WSS) is used as a basic clustering evaluation metric.

## 📷 Visualizations

- **2D Scatter Plot** with colored clusters and centroids.
- **Elbow Curve** to determine optimal `k`.
- **3D Scatter Plot** for multi-dimensional visualization of cluster separation.

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

3. Launch the notebook:
   ```bash
   jupyter notebook k-means-clustering.ipynb
   ```

## 🔍 Example Output

You’ll see:
- Clear 2D clusters with boundaries
- A 3D view revealing spatial separation
- An elbow plot highlighting the optimal number of clusters

## 🛠️ Future Enhancements

- Add support for custom datasets (e.g., upload CSV)
- Integrate silhouette score for better evaluation
- Use PCA for high-dimensional data visualization

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
