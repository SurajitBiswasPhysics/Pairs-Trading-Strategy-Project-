📈 Cointegration-Based Pairs Trading Strategy

This project implements a market-neutral pairs trading strategy based on cointegration and mean reversion. It combines econometric tests, systematic backtesting, transaction cost modeling, and parameter sensitivity analysis to evaluate profitability and robustness.

🔹 Project Overview

Universe: 12 U.S. tech stocks (2020–2025 daily prices, 1403 trading days)

Goal: Identify cointegrated stock pairs, trade mean-reverting spreads, and measure real-world profitability.

Approach:

Pair Selection

Correlation & Engle–Granger cointegration test

ADF test on residuals

Rolling-window stability analysis

Top 5 pairs shortlisted (e.g., MSFT–AMD, MSFT–NVDA, GOOG–CSCO)

Trading Logic

Compute spread & hedge ratio (β)

Generate entry/exit signals from spread z-scores

Backtest with transaction costs (0.05%–0.30% round-trip)

Evaluation

CAGR, Sharpe ratio, annualized volatility

Max drawdown, win rate, trade count

Out-of-sample validation

Sensitivity study over multiple z-entry thresholds

---


## 🙌 About Me

If you're working on financial risk modeling, machine learning, or applied deep learning — let’s connect!

👤 **Surajit Biswas, Ph.D.**  

🔗  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/surajit-biswas-phd/)

📫 surajitbiswas.iiserb@gmail.com

---

## 🏷️ Tags

`Pairs Trading', `Cointegration', `Statistical Arbitrage', `Quant Finance', `Backtesting', `Sharpe Ratio'
