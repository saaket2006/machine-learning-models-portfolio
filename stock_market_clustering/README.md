# Stock Market Clustering

## Problem Statement
This project aims to group different stocks into clusters based on their historical risk and return profiles. By analyzing the `annualized return` and `annualized volatility` (risk), we can identify similar financial instruments within the stock market.

## Dataset
- **Data Source**: `stock_prices_dataset.csv`

The data is preprocessed by calculating daily return percentages, from which we derive the mean return and standard deviation (volatility). These metrics are then annualized assuming 252 trading days. The features are scaled using `StandardScaler`.

## Model Used
- **K-Means Clustering**

## Results
- The Elbow Method was used on `k` values spanning 1 to 10 to empirically establish that `k=4` is the optimal number of clusters.
- Stocks were assigned to 4 distinct clusters. Each cluster is summarized by its count, average annual return, and average annual volatility. Sample stocks belonging to each group are also provided.

## Visualizations
- **Elbow Method Curve**: A line chart plotting the number of clusters (k) against the Within-Cluster Sum of Square (WCSS) to locate the elbow point (`plots/elbow_method.png`).
- **Cluster Scatter Plot**: A 2D visualization plotting Annualized Volatility (X-axis) against Annualized Return (Y-axis), colored by cluster assignment. Cluster centroids are superimposed in red (`plots/stock_clusters.png`).
