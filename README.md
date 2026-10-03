# PCA + K-Means Customer Segmentation

A Machine Learning project that uses **PCA (Principal Component Analysis)** and **K-Means Clustering** to reduce data dimensions and group similar customers.

## 📌 Project Overview

In this project, customer data is first standardized using `StandardScaler`.

Then:

1. Standardize the features
2. Apply PCA to reduce the dimensions to 2 components
3. Check the explained variance
4. Apply K-Means clustering
5. Assign customers to groups
6. Visualize the groups using a PCA scatter plot

## 🧠 Machine Learning Techniques

* StandardScaler
* PCA
* K-Means Clustering
* Dimensionality Reduction
* Unsupervised Learning
* Data Visualization

## 🛠️ Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

## 📂 Project Structure

```text
pca-kmeans-customer-segmentation/
│
├── data/
│   └── customer_data.csv
│
├── PCA_KMeans_Customer_Segmentation.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## 🔄 Project Workflow

```text
Customer Data
      ↓
StandardScaler
      ↓
Scaled Data
      ↓
PCA
      ↓
PCA1 + PCA2
      ↓
K-Means
      ↓
Group 0 / Group 1
      ↓
Visualization
```

## 📊 PCA

PCA is used to reduce multiple features into fewer components while keeping as much of the important variation in the data as possible.

In this project:

```python
PCA(n_components=2)
```

creates two components:

* PCA1
* PCA2

The explained variance ratio is also calculated to see how much variation each component captures.

## 🤖 K-Means

K-Means is an **unsupervised Machine Learning algorithm** used to divide data into groups called clusters.

This project uses:

```python
KMeans(
    n_clusters=2,
    random_state=42,
    n_init=10
)
```

The model assigns each data point to:

* Group 0
* Group 1

## 📈 Visualization

The PCA results are plotted using a scatter plot.

* X-axis: PCA1
* Y-axis: PCA2
* Different groups are displayed separately

## 🎯 What I Learned

Through this project, I practiced:

* Feature scaling
* Dimensionality reduction
* PCA
* Explained variance
* K-Means clustering
* DataFrame filtering
* Group analysis
* Data visualization
* Scikit-Learn workflow

## 🚀 Future Improvements

* Try different numbers of clusters
* Use the Elbow Method to select `k`
* Compare clustering results
* Add more customer features
* Create a more detailed customer segmentation analysis

## 📚 Learning Level

**Machine Learning Roadmap: Level 4 - Advanced Machine Learning**

Topics practiced:

* PCA
* Dimensionality Reduction
* K-Means
* Feature Scaling
* Unsupervised Learning

---

**Built with Python, Pandas, NumPy, Matplotlib and Scikit-Learn.**
