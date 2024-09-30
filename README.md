# Project Overview

This project involves time series analysis and forecasting using several volatility models. The goal is to estimate parameters, evaluate in-sample fits, and compare out-of-sample forecasting performance of different models based on financial data.

## 1. Data Description
The dataset includes:
- Descriptive statistics
- Autocorrelation function (ACF) plots
- Various visualizations

This step provides an overview of the data's structure and statistical properties before fitting any models.

## 2. In-Sample Fit
The following volatility models are estimated using the full sample size:
- AR(1)-RV
- HAR
- HAR-RS
- HAR-Rskew-RKurt
- Realized GARCH
- ARMA-GARCH

Parameters are estimated, and the in-sample fits of these models are compared. Qualitative differences in model estimates are discussed briefly. A plot comparing the in-sample fits of all models is also provided.

## 3. Forecasts
Out-of-sample forecasting performance is evaluated using two forecasting schemes:
1. **Expanding window**: Starting window length of 750, progressively expanding.
2. **Rolling window**: Fixed window length of 750.

Forecast errors are computed for each model. Loss functions (MSE and MAE) are used to compare forecast accuracy. The forecasts are further evaluated statistically using:
- Diebold-Mariano test (based on MSE loss)
- Minzer-Zarnowitz regressions

## 4. Summary
A short summary compares the model performances. It highlights the best in-sample fits, the most accurate forecasting models, and significant statistical findings based on the loss functions and tests.

This project provides insights into the comparative effectiveness of different volatility models in capturing and predicting financial time series data.
