# Pairs Trading Strategy — XOM vs GDX

This project implements a statistical arbitrage strategy based on pair trading between ExxonMobil (XOM) and the Gold Miners ETF (GDX). The strategy uses:

- Cointegration testing (Engle-Granger)
- Regression-based hedge ratio estimation
- Rolling z-score signals
- Mean-reversion logic with realistic transaction costs

## 🔍 Strategy Logic

1. Test for cointegration between two assets
2. Estimate hedge ratio via linear regression
3. Calculate spread: `spread = XOM - hedge_ratio * GDX`
4. Compute rolling z-score of spread
5. Generate trading signals:
   - Short when z-score > 1.5
   - Long when z-score < -1.5
   - Exit when z-score returns within ±0.5
6. Backtest and evaluate using Sharpe Ratio

## 📈 Results

- Time period: Jan 2023 – Jan 2025
- Sharpe Ratio (after transaction costs): **0.57**
- Positive mean-reverting behavior captured with tuned thresholds and regression-based spread construction.

## 🧪 Next Steps

- Automate screener to identify cointegrated pairs
- Dynamically estimate hedge ratio
- Compare with momentum-based strategies

## 🛠 Tech Stack

- Python (pandas, NumPy, yfinance, matplotlib, statsmodels)
- Jupyter Notebook
