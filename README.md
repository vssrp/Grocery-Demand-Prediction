# Grocery Demand Prediction 📈
---

## Overview
This project aims to forecast grocery product demand using historical sales data combined with multiple external factors such as holidays, promotions, and economic indicators. By leveraging machine learning techniques, including the SARIMA model, we predict demand with a focus on optimizing inventory and improving operational efficiency in the retail industry.

---

## Problem Statement
Efficient demand forecasting is a critical challenge for the retail industry, especially in the presence of factors like seasonal variability, promotions, and economic changes. Inaccurate predictions can lead to overstocking, understocking, and financial losses. This project addresses these challenges by integrating diverse datasets to enhance demand prediction accuracy.

---

## Key Features
- **Comprehensive Data Integration**: Combined six datasets, including sales, holidays, promotions, oil prices, transactions, and store details.
- **Exploratory Data Analysis (EDA)**: Detailed analysis of sales trends, promotions, holidays, and economic factors.
- **Machine Learning**: Used the SARIMA model for time-series forecasting to account for seasonal trends and patterns.
- **Error Metrics**: Evaluated model performance using MAE, MSE, and residual analysis.

---

## Dataset Description
[URL for Datasets](https://www.kaggle.com/datasets/siliconx/favoritagrocerysalesforecastingextracted)
1. **sales.csv**: Historical sales data with features like unit sales, item number, store number, and promotion details.  
2. **holidays_events.csv**: Data on national, regional, and local holidays.  
3. **items.csv**: Metadata about items, including categories and perishability.  
4. **oil.csv**: Daily oil prices as an economic indicator.  
5. **stores.csv**: Information on store locations, types, and clusters.  
6. **transactions.csv**: Daily transaction counts at each store.  

---

## Methodology
1. **Data Preprocessing**:
   - Cleaned missing values and retained meaningful features.
   - Addressed data gaps and outliers (e.g., product returns, holiday closures).
2. **Dataset Integration**:
   - Merged datasets on relevant keys like `date`, `store number`, and `item number`.
   - Incorporated holiday and economic indicators to enrich the dataset.
3. **Model Selection**:
   - Implemented SARIMA for its ability to handle time-series data with seasonality.
   - Tuned hyperparameters using grid search for optimal performance.
4. **Model Evaluation**:
   - Evaluated using MAE, MSE, and residual analysis to measure prediction accuracy.

---

## Results
- **Overall Store Forecast**:
  - RMSE: 645.64  
  - MAE: 442.73  
  - MAPE: 7.58%  
- **Top Product Predictions**:
  - Dairy Product: RMSE: 230.71, MAPE: 10.08%  
  - Produce Product: RMSE: 102.16, MAPE: 12.62%  

---

## Future Work
1. **Enhanced Models**:
   - Incorporate advanced neural networks like LSTMs for non-linear relationships.
2. **Expanded Data Scope**:
   - Forecast for all items and stores, instead of a subset.
3. **External Factors**:
   - Include additional economic and competitive factors, such as inflation and competitor pricing.

---

## How to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/grocery-demand-prediction.git
   cd grocery-demand-prediction
