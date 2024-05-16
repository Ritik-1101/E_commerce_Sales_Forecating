# CatBoost Regression for E-commerce Data Analysis

## Description

This project demonstrates the application of CatBoost regression on e-commerce sales data. The workflow includes data loading, preprocessing, feature extraction, clustering, and modeling. The primary goal is to predict daily sales quantities using time series data and CatBoost regression.

## Prerequisites

Before We begin, ensure you have met the following requirements:

- Python 3.x
- Jupyter Notebook

## Installation

### Clone the repository:

```bash
git clone https://github.com/Ritik-1101/E_commerce_Sales_Forecast
cd E_commerce_Sales_Forecast
```
### Install the required packages:


```bash
pip install numpy pandas matplotlib seaborn catboost scikit-learn shap GPyOpt
```


### Load and preprocess data:

- The load_data function loads the e-commerce data from a data.csv file and performs preprocessing steps such as filtering, date extraction, and revenue calculation.

### Analyze stock codes:

- The analyze_stock_codes function processes stock codes to filter and retain valid codes for further analysis.

### Cluster products:

- The cluster_products function clusters products based on their characteristics like median price, median quantities, number of customers, and description length.

### Aggregate daily data:

- The aggregate_daily_data function aggregates the data on a daily basis for modeling.

### Prepare training and validation data:

- The prepare_data function prepares the training and validation datasets based on a specified week.

### CatBoost Model:

- The Catmodel class defines a CatBoost regression model with methods for training, scoring, and visualizing results.

### Hyperparameter Tuning:

- The Hypertuner class uses Bayesian Optimization to find the optimal hyperparameters for the CatBoost model.

### Main function:

- The main function orchestrates the entire workflow, from loading data to hyperparameter tuning and model evaluation.


## Visualizations

The script includes several visualization functions to help interpret the model's performance and feature importance. These visualizations can be viewed in Jupyter Notebook or through saved output files.
Results

The script outputs the model's performance metrics, including RMSE and median absolute error.
Feature importances are visualized using SHAP values.
Monthly RMSE values are calculated and displayed.
The script performs hyperparameter tuning to improve the model's performance.
