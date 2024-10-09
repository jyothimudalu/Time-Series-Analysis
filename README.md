# Time-Series Analysis of USD/INR Exchange Rates

## Overview
This project performs a comprehensive time-series analysis of the USD/INR exchange rate using data gathered from the Federal Reserve Economic Data (FRED) website via the FRED API. The analysis focuses on the exchange rate from January 2014 to June 2024, employing various forecasting models to predict future values.

## Key Components
- **Data Extraction:** The USD/INR exchange rate data is extracted using the FRED API and saved in a CSV format.
- **Data Preprocessing:** The dataset is cleaned and prepared, including handling missing values and setting the appropriate date formats.
- **Stationarity Testing:** The analysis includes tests for stationarity using rolling statistics and the Augmented Dickey-Fuller test.
- **Forecasting Models:** Four different models are applied for forecasting:
  - ARIMA
  - SARIMA
  - LSTM (Long Short-Term Memory)
  - Exponential Smoothing
- **Model Evaluation:** Each model is evaluated using key metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE) to assess their forecasting accuracy.

## Results
The analysis revealed that:
- The ARIMA model outperformed others in terms of accuracy, exhibiting the lowest error metrics.
- The SARIMA model captured seasonality but had higher error rates compared to ARIMA.
- The LSTM model was the least effective for this time series, suggesting that its complexity was not necessary for this dataset.
- Exponential Smoothing provided moderate performance, trailing behind the ARIMA model.

## Requirements
To run this project, you will need the following libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`
- `pmdarima`
- `tensorflow` (for LSTM)
- `fredapi` (for data extraction)

You can install the required packages using:
```bash
pip install pandas numpy matplotlib statsmodels pmdarima tensorflow fredapi
