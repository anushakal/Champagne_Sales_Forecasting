# Champagne Sales Forecasting Using ARIMA and SARIMA
This repository contains the Jupyter Notebook used to forecast monthly champagne sales using ARIMA and SARIMA models. The notebook walks through key steps in time series analysis, including data cleaning, stationarity tests, and fitting different forecasting models.

# Dataset
The dataset used is monthly sales data from Perrin Freres, covering a period from January 1964 to September 1972. The sales data consists of champagne sales (in millions) over this timeframe.
(https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fanupamshah%2Fperrin-freres-monthly-champagne-sales%2Fdata)

# Features
## Data Preprocessing:
Null values are removed, and the sales column is renamed for clarity.
The 'Month' column is converted to a datetime object and set as the index.

## Plot of the sales data after pre-processing:
![image](https://github.com/user-attachments/assets/6167dab1-a4a8-493f-bdba-013d55a4e092)


## Stationarity Check:
An Augmented Dickey-Fuller (ADF) test is performed to check for stationarity.
## Data differencing is used to make the time series stationary.
## Plot of the stationary data:
![image](https://github.com/user-attachments/assets/e9f211d9-effc-4a5a-8959-036e5d85c63f)

# Modeling:
## ARIMA:
AutoRegressive Integrated Moving Average (ARIMA) is used as the primary forecasting model.
Various parameter configurations for p, d, and q are tested after plotting the ACF and PACF values
## Visualizing the ARIMA fitted data:
![image](https://github.com/user-attachments/assets/56505563-26b6-4929-aa8b-2415e54c7213)


## SARIMA:
Seasonal ARIMA (SARIMA) is employed to account for seasonality in the sales data.
The seasonal order of (1, 1, 1, 12) is chosen after observing seasonal patterns.
# SARIMA fitted data:
![image](https://github.com/user-attachments/assets/47a9c904-23c1-4305-9c17-731dbe1cf0cd)


# Future Forecasting:
The model is used to predict sales for future months, extending the dataset beyond the original time frame.
Future dates were generated, and predictions were extended for the next 24 months as shown in the below figure:
![image](https://github.com/user-attachments/assets/c52832d0-9baf-41e9-ab5e-0bd3ddfe7475)


# Results
The final SARIMA model provides better forecasts, considering seasonality in the dataset.


