# Sentiment Analysis

## Problem Statement
The objective of this project is to perform sentiment analysis on textual data to classify sentiments into binary classes: `Positive` (1) and `Negative` (0). 

## Dataset
- **Data Source**: `sentiment_dataset.csv`

The text data is vectorized and transformed using two approaches:
1. `TfidfVectorizer` for the Support Vector Machine (SVM) models.
2. `Tokenizer` and sequence padding for the Neural Network model.

## Model Used
1. **Support Vector Machine (SVM)** (using both `linear` and `rbf` kernels).
2. **Neural Network (Feed-Forward)** built with TensorFlow/Keras (Embedding layer, GlobalAveragePooling1D, Dense, and Dropout).

## Results
- **SVM**: Achieved accuracy, ROC AUC scores, confusion matrices, and classification reports for both `linear` and `rbf` kernels. 
- **Neural Network**: Trained over 10 epochs using binary cross-entropy loss, reporting final test accuracy and loss.

## Visualizations
- **SVM Confusion Matrices**: Heatmaps representing True/False Positives and Negatives for both kernels (`svm_confusion_matrix_linear.png`, `svm_confusion_matrix_rbf.png`).
- **ROC Curves**: Receiver Operating Characteristic curves plotted for both SVM models (`svm_roc_curve_linear.png`, `svm_roc_curve_rbf.png`).
- **SVM Decision Boundary**: Visualized the Linear SVM decision boundary on a 2D PCA-reduced subset of the training data (`svm_decision_boundary_pca.png`).
- **Training Graphs**: Plotted the training vs validation Accuracy (`nn_accuracy_plot.png`) and Loss (`nn_loss_plot.png`) across epochs for the Neural Network.
