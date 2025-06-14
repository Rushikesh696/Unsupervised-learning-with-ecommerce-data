# Customer Segmentation using RFM Analysis, K-Means Clustering & PCA
### Project Overview
This project focuses on Customer Segmentation using Unsupervised Learning techniques on an Online Retail dataset. The primary goal is to identify customer groups based on their purchasing behavior using RFM (Recency, Frequency, Monetary) analysis.

To uncover meaningful patterns, the project implements:

RFM Scoring

K-Means Clustering

Principal Component Analysis (PCA) for dimensionality reduction and better visualization

### Technologies Used
Python

Pandas – data manipulation

Matplotlib / Seaborn – data visualization

Scikit-learn – KMeans, PCA, scaling

Jupyter Notebook / Colab – development environment

### Steps Performed
1. Data Preprocessing
Removed missing CustomerID entries.

Filtered out cancelled transactions (InvoiceNo starting with 'C').

Calculated TotalPrice = Quantity * UnitPrice.

2. RFM Analysis
Recency: Days since the last purchase.

Frequency: Number of transactions.

Monetary: Total amount spent.

Customers were scored on each RFM metric to form an overall RFM score.

3. RFM Segmentation
Created RFM segments by quantile binning (e.g., using .qcut()).

Assigned customer segments like "Champions", "Loyal", "At Risk", etc.

4. K-Means Clustering
Scaled RFM values using StandardScaler.

Used Elbow Method to find the optimal number of clusters (k).

Applied K-Means clustering on the scaled RFM features.

5. PCA (Principal Component Analysis)
Reduced the feature space to 2D for visualization.

Plotted the clusters in PCA space for interpretation.

### Results
Identified distinct customer segments based on their purchase behavior.

K-Means effectively grouped customers with similar RFM scores.

PCA helped visualize the clusters and validate the separation.

Business can now target high-value customers, re-engage at-risk customers, and customize marketing strategies.

### Key Learnings
RFM analysis is a powerful method for quantifying customer behavior.

K-Means is effective for segmenting customers when combined with proper feature engineering.

PCA enhances interpretability in high-dimensional clustering problems.

Preprocessing and feature scaling significantly impact unsupervised learning performance.

### Conclusion
This project demonstrates how unsupervised learning techniques can provide actionable business insights from raw retail data. Through a combination of RFM modeling, K-Means clustering, and PCA visualization, customer behavior was segmented efficiently. These insights enable businesses to make data-driven marketing decisions, improve customer retention, and boost overall sales performance.
