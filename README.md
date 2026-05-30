# Nifty-50 Future Prediction using ARIMA & Monte Carlo

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![Stars](https://img.shields.io/github/stars/divyankm/Nifty-50-Future-Prediction-using-Arima?style=social)

Forecasting the **NIFTY 50 index** up to **10 years ahead** using ARIMA time series modelling and Monte Carlo simulations. Built on monthly OHLC data spanning 2003–2021.

---

## 📊 What is NIFTY 50?

The NIFTY 50 is India's benchmark stock market index — a weighted average of the 50 largest companies listed on the National Stock Exchange (NSE). It is one of the two primary indices used in India, alongside BSE SENSEX, and was launched on 22 April 1996.

---

## 📁 Repository Structure

```
├── Nifty_50_Future_Prediction.ipynb   ← ARIMA model: 10-year price forecast
├── Nifty_MC_Algo.ipynb                ← Monte Carlo simulation on Nifty 50
├── INFY_MC.ipynb                      ← Monte Carlo simulation on Infosys stock
├── Nifty_monthly_OHLC.xlsx            ← Dataset: monthly OHLC (2003–Mar 2021)
└── README.md
```

---

## 🔬 Notebooks

### 1. `Nifty_50_Future_Prediction.ipynb` — ARIMA Forecasting
- Loads monthly NIFTY 50 OHLC data from 2003 to March 2021
- Performs stationarity tests (ADF test)
- Fits an ARIMA model to the closing price series
- Forecasts NIFTY 50 price for the **next 10 years**
- Plots forecast with confidence intervals

### 2. `Nifty_MC_Algo.ipynb` — Monte Carlo Simulation (Nifty 50)
- Simulates thousands of possible future price paths using Geometric Brownian Motion
- Estimates probability distribution of future NIFTY 50 prices
- Visualises best-case, worst-case, and expected price scenarios

### 3. `INFY_MC.ipynb` — Monte Carlo Simulation (Infosys)
- Applies the same Monte Carlo framework to Infosys (INFY) stock
- Compares individual stock volatility vs index behaviour

---

## 📦 Dataset

| File | Source | Period | Frequency |
|------|--------|--------|-----------|
| `Nifty_monthly_OHLC.xlsx` | [Investing.com](https://in.investing.com/indices/s-p-cnx-nifty-historical-data) | 2003 – Mar 2021 | Monthly |

---

## 🛠️ Tech Stack

- **Python** — pandas, numpy, matplotlib, statsmodels
- **ARIMA** — statsmodels `ARIMA` for time series forecasting
- **Monte Carlo** — Geometric Brownian Motion simulation
- **Jupyter Notebook**

---

## 📚 References

- [Time Series for Beginners with ARIMA — Kaggle](https://www.kaggle.com/freespirit08/time-series-for-beginners-with-arima)
- [Monte Carlo Simulations for Stock Prices — Analytics Vidhya](https://medium.com/analytics-vidhya/monte-carlo-simulations-for-predicting-stock-prices-python-a64f53585662)
- [Finance Portfolio with Monte Carlo — GitHub](https://github.com/eliasmelul/finance_portfolio)
- [Monte Carlo for Stock Prices — DataSciencePlus](https://datascienceplus.com/how-to-apply-monte-carlo-simulation-to-forecast-stock-prices-using-python/)
