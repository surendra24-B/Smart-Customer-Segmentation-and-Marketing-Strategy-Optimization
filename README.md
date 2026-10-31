# Customer Segmentation Using K-Means Clustering

## Project Overview

Developed a customer segmentation model using **Unsupervised Machine Learning** to group mall customers based on age, annual income, and spending behaviour. Applied K-Means clustering to identify distinct customer segments and generate actionable business insights for targeted marketing strategies.

## Objectives

- Identify customer groups with similar characteristics.
- Analyse customer income and spending patterns.
- Determine the optimal number of clusters.
- Understand customer behaviour through data visualization.
- Provide business recommendations for targeted marketing.

## Technologies Used

- **Programming Language:** Python
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Algorithm:** K-Means Clustering
- **Dimensionality Reduction:** PCA
- **Development Environment:** Jupyter Notebook

## Dataset Description

The project uses a Mall Customers dataset containing 200 customer records.

| Feature | Description |
|---|---|
| CustomerID | Unique customer identifier |
| Gender | Customer gender |
| Age | Customer age |
| Annual Income (k$) | Annual customer income |
| Spending Score (1-100) | Customer spending behaviour score |

## Project Workflow

1. Data Loading and Exploration
2. Exploratory Data Analysis (EDA)
3. Data Preprocessing
4. Feature Selection
5. Feature Scaling using StandardScaler
6. Optimal Cluster Selection using Elbow Method
7. Model Evaluation using Silhouette Score
8. K-Means Clustering
9. Cluster Visualization and Profiling
10. PCA-based Visualization
11. New Customer Cluster Prediction

## Model Optimization

Evaluated different cluster configurations using the Silhouette Score.

| Number of Clusters (K) | Silhouette Score |
|---|---:|
| 2 | 0.3563 |
| 3 | 0.3628 |
| 4 | 0.4092 |
| **5** | **0.4281** |
| 6 | 0.4216 |
| 7 | 0.4126 |
| 8 | 0.3947 |
| 9 | 0.3830 |
| 10 | 0.3589 |

**Selected K = 5**, which achieved the highest Silhouette Score among the tested configurations.

## Customer Segments Identified

The model identified five customer segments:

1. **Cluster 0:** Medium-to-high income customers with moderate spending behaviour.
2. **Cluster 1:** Low-income customers with high spending behaviour.
3. **Cluster 2:** High-income customers with high spending behaviour.
4. **Cluster 3:** Low-income customers with low spending behaviour.
5. **Cluster 4:** High-income customers with low spending behaviour.

## Business Applications

- Develop targeted marketing campaigns.
- Identify potentially valuable customer segments.
- Improve customer engagement and retention.
- Design personalized offers and loyalty programmes.
- Understand customer spending patterns.

## Installation and Execution

### 1. Clone the Repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the Project Directory

```bash
cd Customer-Segmentation-Using-KMeans
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Load the Dataset

```python
import pandas as pd

df = pd.read_csv("mall_customers.csv")

print(df.head())
```

### 6. Execute the Notebook

Run the notebook cells sequentially to perform data analysis, clustering, evaluation, and visualization.

## Key Findings

- Identified five distinct customer segments.
- Achieved a maximum Silhouette Score of 0.4281.
- Observed different spending behaviours across income groups.
- Generated actionable customer segmentation insights.

## Future Improvements

- Implement Hierarchical Clustering and DBSCAN.
- Compare multiple clustering algorithms.
- Build an interactive customer segmentation dashboard.
- Explore additional customer behavioural features.

## Author

**Surendra Boddapu**

Aspiring Data Scientist | Machine Learning Enthusiast

---

*This project demonstrates the application of unsupervised machine learning to
