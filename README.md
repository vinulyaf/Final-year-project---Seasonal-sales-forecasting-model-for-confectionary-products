Demand Forecasting for FMCG Confectionery Products
Overview
This project develops a multi-model time-series forecasting framework to predict monthly demand for confectionery products across different regions. The objective is to improve demand planning by generating accurate, disaggregated forecasts at the Region × Candy Type level.
Four forecasting approaches were implemented and compared:


SARIMA


Holt-Winters Exponential Smoothing


LSTM (Baseline)


LSTM (Tuned using Keras Tuner)



Key Objective
To identify the most accurate forecasting model for each product-region combination and generate six-month ahead demand forecasts (Jan–Jun 2026) to support operational decision-making.

⚙️ Methodology
1. Data Preparation


Monthly sales data aggregated by Region × Candy Type


Minimum series length: 24 months


Missing values handled using time-based interpolation


2. Train-Test Split - 80/20


3. Models Implemented
SARIMA


ADF test used to determine differencing (d)


ACF/PACF used for parameter identification


Seasonal component fixed at 12 months


EWMA pre-smoothing applied for stability


Holt-Winters


Exhaustive search across valid configurations:


Trend: additive, multiplicative, none


Seasonality: additive, multiplicative


Damped trend + Box-Cox options




Best model selected using AIC


LSTM (Baseline)


2-layer stacked architecture:


LSTM(64) → Dropout → LSTM(32) → Dense




12-month lookback window


MinMax scaling applied


🔹 LSTM (Tuned)


Bayesian optimisation (Keras Tuner)


Tuned parameters:


Number of layers (1–3)


Units (32–256)


Dropout (0.1–0.5)


Learning rate




Evaluation Metrics
Models were evaluated on the test set using:


MAPE (primary metric)


RMSE


MAE


Best model per combination selected based on minimum MAPE.

