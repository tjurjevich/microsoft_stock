# Project Summary

This project explores a handful of models to apply against daily closing Microsoft (MSFT) stock prices from 2015 thru 2021. ARIMA/SARIMA models are initially fit, however, diagnostic checks fail due to heteroscedasticity and non-normality within residuals. A GARCH component is added to hopefully account for high variance, however, this doesn't help model residuals conform to ARIMA assumptions.

A second subset of models are explored, with these being centered around deep learning and a neural network architecture.
  1. **Multilayer Perceptron (MLP)**
  2. **Long Short Term Memory (LSTM)**
  3. **Recurrent Neural Network (RNN)**
  4. **Gated Recurrent Unit (GRU)**

The GRU model holds up the best of these four model types (MAE: 3.4, MSE: 19.9, MAPE: 1.7%), followed up by LSTM, MLP, and finally, RNN.

Although not explored in this mini project, future daily closing stock prices could be obtained (via `yfinance` module) in order to compare GRU model forecasts against true values.
