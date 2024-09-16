# Champagne Sales Forecasting Using ARIMA and SARIMA
This repository contains the Jupyter Notebook used to forecast monthly champagne sales using ARIMA and SARIMA models. The notebook walks through key steps in time series analysis, including data cleaning, stationarity tests, and fitting different forecasting models.

# Dataset
The dataset used is monthly sales data from Perrin Freres, covering a period from January 1964 to September 1972. The sales data consists of champagne sales (in millions) over this timeframe.

# Features
## Data Preprocessing:
Null values are removed, and the sales column is renamed for clarity.
The 'Month' column is converted to a datetime object and set as the index.

## Plot of the sales data after pre-processing:
![image](https://github.com/user-attachments/assets/6167dab1-a4a8-493f-bdba-013d55a4e092)


## Stationarity Check:
An Augmented Dickey-Fuller (ADF) test is performed to check for stationarity.
Data differencing is used to make the time series stationary.

# Modeling:
## ARIMA:
AutoRegressive Integrated Moving Average (ARIMA) is used as the primary forecasting model.
Various parameter configurations for p, d, and q are tested.

## SARIMA:
Seasonal ARIMA (SARIMA) is employed to account for seasonality in the sales data.
The seasonal order of (1, 1, 1, 12) is chosen after observing seasonal patterns.

# Future Forecasting:
The model is used to predict sales for future months, extending the dataset beyond the original time frame.
Results
The final SARIMA model provides better forecasts, considering seasonality in the dataset.
Future dates were generated, and predictions were extended for the next 24 months.
Visualizations
The notebook includes various plots:

Time series visualization of champagne sales.
ACF and PACF plots for identifying ARIMA parameters.
Forecasted sales overlaid on actual sales data.
Contact
For any questions or issues, please contact your-email@example.com.


