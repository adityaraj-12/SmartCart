# SmartCart — E-commerce Customer Segmentation

## 📌 Overview

**SmartCart** is an unsupervised machine learning project that segments e-commerce customers into meaningful groups based on their purchasing behavior.

The project uses **customer transaction data** and clustering techniques to identify different customer segments. These segments can help businesses understand customer behavior, improve marketing strategies, personalize offers, and make better business decisions.

## 🎯 Objectives

* Analyze e-commerce customer purchasing behavior.
* Perform data cleaning and exploratory data analysis.
* Identify important customer characteristics.
* Apply feature engineering to prepare data for clustering.
* Use **unsupervised learning** to group similar customers.
* Determine the optimal number of customer clusters.
* Visualize and interpret the resulting customer segments.
* Generate actionable business insights from the clusters.

## 🧠 Machine Learning Approach

The project follows the following pipeline:

```text
Customer Dataset
       ↓
Data Cleaning
       ↓
Exploratory Data Analysis
       ↓
Feature Engineering
       ↓
Feature Scaling
       ↓
Clustering
       ↓
Cluster Evaluation
       ↓
Customer Segmentation
       ↓
Business Insights
```

## 📊 Dataset

The project uses an **e-commerce customer/transaction dataset** containing information related to customer purchasing activity.

Typical attributes may include:

* Customer ID
* Year_Birth 
* Education 
* Marital_status
* Income
* Kidhome
* Teenhome
* Dt_Customer
* MntWines
* MntFruits 
* MntMeatProducts 
* MntFishProducts
* MntSweetProducts
* MntGoldProds
* TeenhNumDealsPurchasesome
* NumWebPurchases 
* NumCatalogPurchases
* NumStorePurchases
* NumWebVisitsMonth 
* Recency
* Complain 


The raw transaction-level data is transformed into customer-level features before applying clustering.

## 🔧 Feature Engineering

Customer behavior is represented using meaningful numerical features such as:

### Recency

Number of days since the customer's most recent purchase.

### Frequency

Number of purchases/orders made by the customer.

### Monetary Value

Total amount spent by the customer.

These features form an **RFM (Recency, Frequency, Monetary)** representation of customer behavior.

Additional features can also be included depending on the dataset.

## 🤖 Clustering Algorithm

### K-Means Clustering

The primary clustering algorithm used in SmartCart is **K-Means**.

K-Means divides customers into `K` groups by minimizing the distance between customers and their respective cluster centers.

The algorithm follows these general steps:

1. Select the number of clusters `K`.
2. Initialize cluster centroids.
3. Assign each customer to the nearest centroid.
4. Recalculate the centroids.
5. Repeat until the clusters stabilize.

## 📐 Selecting the Number of Clusters

The optimal number of clusters can be determined using:

### Elbow Method

The Elbow Method analyzes the **Within-Cluster Sum of Squares (WCSS)** for different values of `K`.

### Silhouette Score

The Silhouette Score measures how well-separated and internally consistent the clusters are.

A higher silhouette score generally indicates better-defined clusters.

## 📈 Visualization

The project uses visualizations to understand customer segments, including:

* Distribution plots
* Correlation heatmaps
* Elbow curves
* Silhouette analysis
* Cluster scatter plots
* Customer segment distributions
* Feature-wise cluster comparisons

Dimensionality reduction techniques such as **PCA** can also be used to visualize high-dimensional customer data in two dimensions.

## 🏷️ Customer Segments

After clustering, the groups can be interpreted according to their purchasing behavior.

Example segments may include:

| Segment                 | Characteristics                             |
| ----------------------- | ------------------------------------------- |
| 🏆 High-Value Customers | High spending and frequent purchases        |
| 💎 Loyal Customers      | Frequent purchases with consistent activity |
| 🛒 Regular Customers    | Moderate purchasing activity                |
| 🌱 New/Recent Customers | Recent purchases but limited history        |
| ⚠️ At-Risk Customers    | Long time since last purchase               |
| 💤 Low-Value Customers  | Low spending and low purchase frequency     |

> The actual cluster names and characteristics depend on the dataset and clustering results.

## 🛠️ Technologies Used

* **Python**
* **Pandas** — Data manipulation
* **NumPy** — Numerical computation
* **Matplotlib** — Data visualization
* **Seaborn** — Statistical visualization
* **Scikit-learn** — Machine learning and clustering
* **Jupyter Notebook** — Development and analysis

## 📁 Project Structure

```text
SmartCart/
│
├── smartcart_customers.csv
│   
├── SmartCart_Customer_Segmentation.ipynb
│
└── README.md
```

## 📦 Requirements

Example `requirements.txt`:

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
jupyter
```

## 💡 Business Applications

Customer segmentation can help e-commerce businesses:

* Create personalized marketing campaigns.
* Identify high-value customers.
* Improve customer retention.
* Target inactive or at-risk customers.
* Recommend suitable products and offers.
* Optimize promotional strategies.
* Understand different purchasing patterns.
* Improve customer lifetime value.

## 🔮 Future Improvements

Potential improvements include:

* Testing different clustering algorithms such as DBSCAN and Hierarchical Clustering.
* Applying PCA or other dimensionality reduction techniques.
* Creating an interactive **Streamlit dashboard**.
* Adding customer lifetime value analysis.
* Building personalized recommendation strategies.
* Automating customer segmentation for new transactions.
* Comparing clustering performance using multiple evaluation metrics.

## 📌 Key Learning Outcomes

Through this project, the following concepts are demonstrated:

* Unsupervised Machine Learning
* Customer Segmentation
* RFM Analysis
* K-Means Clustering
* Feature Engineering
* Data Preprocessing
* Feature Scaling
* Exploratory Data Analysis
* Elbow Method
* Silhouette Score
* PCA Visualization
* Business-oriented ML interpretation

## 👨‍💻 Author

Adityaraj

M.Tech — Artificial Intelligence & Data Science

---

⭐ If you find this project useful, consider giving the repository a star!
