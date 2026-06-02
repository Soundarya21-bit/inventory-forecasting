# Inventory Forecasting Analysis
 
**Demand Forecasting using Time Series (ARIMA & Prophet) — Client Project**
 
This project forecasts future inventory demand for a real client using
historical sales data and time series techniques.
 
---
 
## Project Overview
 
The business goal was to optimize stock planning and reduce
procurement inefficiencies. I built forecasting models to predict
product demand for upcoming weeks across multiple SKUs.
 
---
 
## Dataset
  
- Features: Date, Product ID, Historical Sales/Inventory Data
- Target: Next_Inventory_Quantity
- Size: 2 years of historical sales data across 50+ product SKUs
 
---
 
## Tools & Libraries
 
- Python
- Pandas, NumPy
- Scikit-learn
- Statsmodels (ARIMA)
- Prophet (Facebook)
- Matplotlib / Seaborn
- MySQL + SQLAlchemy (database integration)
 
---
 
## Approach
 
1. Performed time series decomposition to identify Trend,
   Seasonality, and Residual components
2. Validated stationarity using ADF (Augmented Dickey-Fuller) test
3. Applied differencing to achieve stationarity where needed
4. Built and compared ARIMA and Prophet models
5. Evaluated using RMSE and MAPE metrics
6. Integrated pipeline with MySQL via SQLAlchemy
 
---
 
## Models Used
 
- ARIMA (AutoRegressive Integrated Moving Average) ✅ Final Model
- Prophet (Facebook) — compared alongside ARIMA
 
---
 
## Final Model Performance
 
| Metric | ARIMA | Prophet |
|--------|-------|---------|
| RMSE   | ~12.8 | Higher  |
| MAPE   | ~11.4%| Higher  |
 
- **Selected Model**: ARIMA
- **MAPE reduced by ~12% vs client's existing forecasting method**
- Best suited for capturing seasonality and trend in time-series data
 
---
 
## Key Results
 
- Reduced forecast error (MAPE) by 12% compared to client's existing method
- ARIMA outperformed Prophet on this dataset
- Delivered actionable demand planning report to client stakeholder
- Integrated with MySQL for automated data retrieval and storage
 
---
 
## Files
 
- `Inventory_Forecasting_Analysis_Final.ipynb` — Full notebook with
  EDA, ADF test, ARIMA modeling, Prophet comparison, MAPE/RMSE evaluation
 
---
 
## Summary
 
ARIMA performed best for this time series forecasting task. The model
captured seasonality and trend effectively and reduced MAPE by 12%
compared to the client's existing forecasting method, enabling better
inventory planning decisions.
