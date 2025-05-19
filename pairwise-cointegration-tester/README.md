# Cointegration Screener Tool

This project implements a pairwise cointegration screener to identify statistically significant trading pairs based on long-term equilibrium relationships. It is inspired by statistical arbitrage strategies often used in quant finance.

## 🔍 What It Does

- Accepts a list of stock or ETF tickers
- Downloads historical price data via Yahoo Finance
- Calculates Engle-Granger cointegration p-values for all unique ticker pairs
- Outputs a ranked list of the most cointegrated pairs

## 🧠 Key Concepts

**Cointegration** is a statistical property where two non-stationary time series have a linear combination that is stationary — meaning the spread between them tends to revert to a mean. This is crucial for building mean-reversion strategies like pairs trading.

## 📦 Requirements

- Python 3.x
- `pandas`
- `numpy`
- `statsmodels`
- `yfinance`
- `matplotlib` (optional for plotting)


## 🚀 How to Use

1. Modify the `tickers` list in `screener.ipynb`
2. Run the notebook to compute p-values
3. Review the sorted table of ticker pairs with the lowest p-values

