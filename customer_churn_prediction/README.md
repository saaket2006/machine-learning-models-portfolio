# Customer Churn Prediction

## Problem Statement
The goal of this project is to predict whether a customer will churn (cancel their service) based on their account details, usage patterns, and subscription plans (e.g., International plan, Voice mail plan).

## Dataset
- **Training Data**: `churn-train.csv`
- **Testing Data**: `churn-test.csv`

## Model Used
The following machine learning models were used for prediction:
1. **Logistic Regression**
2. **Random Forest Classifier** (optimized using GridSearchCV for hyperparameter tuning)

## Results
- **Logistic Regression**: Evaluated using Accuracy, Precision, Recall, and Odds Ratios.
- **Random Forest**: Evaluated using Accuracy, Precision, Recall, and F1-Score on the test set. The `GridSearchCV` method determined the best combination of parameters (e.g., `n_estimators`, `max_depth`, `min_samples_split`).

## Visualizations
- **ROC Curve**: Computed and plotted for the Logistic Regression model (`logistic_regression_roc.png`), highlighting the True Positive Rate vs False Positive Rate in order to evaluate the area under the curve.
- **Feature Importance**: Generated a bar chart based on the best Random Forest model, showing the importance of each feature in predicting churn (`random_forest_feature_importance.png`).
