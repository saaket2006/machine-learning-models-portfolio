# Iris Species Classification

## Problem Statement
The goal of this project is to classify iris flowers into their correct species based on their morphological characteristics: `sepal_length`, `sepal_width`, `petal_length`, and `petal_width`.

## Dataset
- **Data Source**: `iris_dataset.csv`

## Model Used
This project explores two classification algorithms:
1. **Decision Tree Classifier** (Standard Model and Pruned Model to prevent overfitting)
2. **K-Nearest Neighbors (KNN)** (Evaluating for multiple `K` values)

## Results
- **Decision Trees**: Evaluated the standard tree versus a pruned tree using Accuracy and weighted F1-score to observe the impact of controlling max depth and leaf samples.
- **KNN**: Evaluated the model using Accuracy, Precision, Recall, and a Confusion Matrix. Iterated over `K` values from 1 to 20 to find the optimal number of neighbors yielding maximum accuracy.

## Visualizations
- **Decision Tree Structures**: Plotted and saved both the standard (`decision_tree.png`) and pruned decision trees (`pruned_decision_tree.png`) using `sklearn.tree.plot_tree`.
- **KNN Accuracy vs K Value**: Created a line plot comparing test set accuracy against different `K` values (`knn_k_comparison.png`) to visually verify the optimal `K`.
