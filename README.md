# Housing-Price-Prediction

This repository contains a machine learning project aimed at predicting housing prices using the **Boston Housing Dataset**. The goal is to use different regression models to estimate housing prices and compare their performances based on various metrics.

## Project Overview

The main objective of this project is to explore and implement various regression models for predicting the median value of homes (`medv`) in Boston, using features such as crime rate, number of rooms, accessibility to highways, and other socio-economic factors.

### Models Used:
- **Linear Regression**
- **Decision Tree**
- **Support Vector Regression (SVR)**

Each model is evaluated using cross-validation and then further tested using a holdout test set. Performance metrics such as RMSE, MAE, MSE, and R² score are used to compare the models.

## Dataset

The dataset used in this project is the **Boston Housing Dataset**. It includes 14 features, some of which are:

- **CRIM**: Crime rate by town.
- **ZN**: Proportion of residential land zoned for large lots.
- **INDUS**: Proportion of non-retail business acres.
- **RM**: Average number of rooms per dwelling.
- **AGE**: Proportion of owner-occupied units built prior to 1940.
- **TAX**: Full-value property tax rate per $10,000.

**Target Variable:**
- **MEDV**: Median value of owner-occupied homes in $1000s.

## Project Steps

1. **Data Preprocessing**
   - Checked for missing values and cleaned the dataset.
   - Standardized the feature set for better model performance.
   
2. **Exploratory Data Analysis**
   - Generated correlation heatmaps and scatter plots to visualize relationships between features and the target variable.

3. **Modeling**
   - Implemented Linear Regression, Decision Tree, and Support Vector Regression models.
   - Evaluated models using 5-fold cross-validation.

4. **Model Evaluation**
   - Used metrics like **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, and **R² Score** to assess model performance.

## Results

The following table summarizes the performance of each model:

| Model                    | MAE  | MSE  | RMSE | R²   |
|---------------------------|------|------|------|------|
| Linear Regression          | 3.19 | 24.29| 4.93 | 0.67 |
| Decision Tree              | 2.51 | 10.93| 3.31 | 0.85 |
| Support Vector Regression  | 2.73 | 25.69| 5.07 | 0.65 |

The **Decision Tree** model performed the best based on **RMSE** and **R²**.

## Visualization

The project also includes visualizations such as:
- **Heatmap** of feature correlations.
- **Scatter plots** showing relationships between features and housing prices.
- **Bar plot** comparing models based on their R² scores.

## Installation and Requirements

To run this project, you'll need the following libraries installed:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
