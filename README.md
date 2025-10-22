AirPassengers: Time‑Series Forecasting with SARIMA and LSTM

Overview
Forecast monthly airline passengers (1949–1960) with classical models (Seasonal Naive, Holt‑Winters, SARIMA) and a small LSTM. Includes clean splits, clear metrics, and comparison plots.

Data

File: data/air_passengers.csv with columns:

Month (YYYY‑MM)

Passengers (integer)

Quick start

Python 3.10+

pip install -r requirements.txt

Open notebooks in notebooks/:

01_explore_decompose.ipynb (visualize, STL)

02_baselines_holtwinters.ipynb (baselines + Holt‑Winters)

03_sarima_tuning.ipynb (SARIMA with m=12)

04_lstm_forecasting.ipynb (LSTM with lookback=24)

Evaluation

Splits: Train 1949–1957, Val 1958–1959, Test 1960

Metrics: RMSE, MAE, MAPE

Baseline: Seasonal‑naive (t uses t‑12)

Deliverables

Forecast plots (baseline, SARIMA, LSTM)

Residual and ACF/PACF diagnostics

Metric table comparing models
