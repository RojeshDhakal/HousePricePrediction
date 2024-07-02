# House Price Prediction Project

## Overview
This project aims to predict house prices using the Ames Housing dataset from Kaggle. Various regression techniques, including Linear Regression and Lasso Regression, are employed and evaluated for their performance.

## Dataset
The dataset used is sourced from Kaggle.com, which contains various features related to residential homes in Ames, Iowa. The target variable is `SalePrice`, representing the sale price of the house.

## Preprocessing
- Missing Values: Handled missing values in numerical columns by imputing with mean values.
- Dropping Columns: Removed columns with high missing values and low information content.

## Model Building
Two regression models were implemented:
- **Linear Regression**: Utilized as a baseline model for predicting house prices.
- **Lasso Regression**: Applied L1 regularization to potentially improve generalization.

## Evaluation
Performance metrics used to evaluate models:
- Mean Squared Error (MSE): Measures the average squared difference between predicted and actual values.
- R-squared (R²): Indicates the proportion of the variance in the dependent variable that is predictable from the independent variables.

## Results
- **Linear Regression**: Achieved a training score of 0.807 and a testing score of 0.823.
- **Lasso Regression**: Tuned with cross-validation, yielding an optimal alpha of 60.10 and a testing score of 0.823.


## Dependencies
- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn

## Results

### Linear Regression
- **Training Score**: 0.807
- **Testing Score**: 0.823
- **Mean Squared Error (MSE)**: 1,356,492,637.95
- **R-squared (R²)**: 0.823

### Lasso Regression (with Cross-Validation)
- **Optimal Alpha**: 60.10
- **Testing Score**: 0.823
- **Mean Squared Error (MSE)**: 1,355,652,187.80
- **R-squared (R²)**: 0.823

Both models, Linear Regression and Lasso Regression, achieved comparable performance on the test dataset with an R-squared score of 0.823, indicating that approximately 82.3% of the variance in house prices can be explained by the features included in the models. Lasso Regression, after tuning with cross-validation to find the optimal regularization parameter (alpha), did not significantly outperform the baseline Linear Regression in this case.

These results suggest that while both models provided reasonable predictions for house prices based on the given dataset, further exploration of feature engineering, model tuning, or trying different algorithms could potentially enhance predictive accuracy.
