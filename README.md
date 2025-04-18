# Clustering Evaluation with Multiple Metrics

This repository implements multiple clustering algorithms on the Iris dataset and evaluates their performance using three different clustering evaluation metrics:
- **Silhouette Score**
- **Calinski-Harabasz Index**
- **Davies-Bouldin Index**

### Clustering Algorithms Implemented:
1. **Spectral Clustering**
2. **Gaussian Mixture Model (GMM)**
3. **Fuzzy C-Means**

### Data Preprocessing Techniques:
The following data preprocessing methods are applied:
1. **Standard Scaling**
2. **Min-Max Scaling**
3. **Normalization**

The preprocessing methods are applied to the Iris dataset, and the clustering algorithms are evaluated on various cluster numbers (3, 5, and 7).

### Evaluation Metrics:
The clustering results are evaluated using three metrics:
1. **Silhouette Score**: Measures how similar an object is to its own cluster compared to other clusters. The higher the value, the better.
2. **Calinski-Harabasz Index**: Measures the ratio of the sum of between-cluster dispersion to within-cluster dispersion. Higher values are better.
3. **Davies-Bouldin Index**: Measures the average similarity between each cluster and its most similar one. Lower values indicate better clustering.

### Code Summary:
- **Preprocessing**: The data is preprocessed using Standard Scaling, Min-Max Scaling, and Normalization.
- **Clustering**: Spectral Clustering, GMM, and Fuzzy C-Means are applied to the data.
- **Evaluation**: Each clustering result is evaluated using the three mentioned metrics.

### Best Results:

#### Best Silhouette Score Result:
```
Algorithm                   GMM
Preprocessing        normalized
Clusters                      3
Silhouette             0.644711
Calinski-Harabasz    888.347519
Davies-Bouldin         0.983528
```

#### Best Calinski-Harabasz Index Result:
```
Algorithm            Spectral Clustering
Preprocessing                 normalized
Clusters                               3
Silhouette                      0.572519
Calinski-Harabasz            1428.385072
Davies-Bouldin                  0.654138
```

#### Best Davies-Bouldin Index Result:
```
Algorithm            Spectral Clustering
Preprocessing                 normalized
Clusters                               3
Silhouette                      0.572519
Calinski-Harabasz            1428.385072
Davies-Bouldin                  0.654138
```

### Requirements:
To run this code, ensure the following packages are installed:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `skfuzzy`

You can install the required packages using pip:

```
pip install numpy pandas matplotlib seaborn scikit-learn skfuzzy
```

### How to Run:
1. Clone the repository to your local machine.
2. Install the necessary dependencies.
3. Run the `clustering.py` file (or your respective script) to see the clustering results and evaluation metrics.

### Visualizations:
The clustering results for each algorithm are visualized using PCA (Principal Component Analysis) for dimensionality reduction. Each algorithm’s result is plotted with a different number of clusters (3, 5, and 7) to give a visual understanding of the clustering quality.

---

Let me know if you need further changes!
