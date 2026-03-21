# House Price Prediction

## Problem Statement
The objective of this project is to predict the median value of owner-occupied homes (MEDV) based on various features such as crime rate, number of rooms, and accessibility to highways.

## Dataset
- **Data Source**: `house_prediction_dataset.csv`

The dataset is preprocessed by handling missing values (imputed using the median) and standardizing numerical features using `StandardScaler`.

## Model Used
- **Simple Linear Regression**

## Results
The performance of the model is evaluated on both the training (80%) and testing (20%) datasets. 
Metrics calculated include:
- **R-squared ($R^2$) Score**: To measure the proportion of variance explained by the model.
- **Mean Squared Error (MSE)**: To evaluate the average squared difference between true and predicted values.
Model Interpretability is supported by analyzing the coefficients and the baseline intercept.

## Visualizations
- **Actual vs Predicted Scatter Plot**: A visualization of the `True Values (MEDV)` against `Predicted Values (MEDV)` on the test set. A red dashed reference line indicates a perfect prediction, helping visually assess model accuracy.
