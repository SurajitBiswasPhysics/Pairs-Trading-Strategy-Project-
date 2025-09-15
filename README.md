# 📈 Statistical Arbitrage: Pairs Trading Strategy

This project implements a **statistical arbitrage (pairs trading) strategy** using a universe of US tech stocks. The goal was to **identify, rank, and backtest mean-reverting stock pairs** that exhibit strong co-movement, and evaluate their profitability both in-sample and out-of-sample.

---

## 🎯 Project Objective
- Detect cointegrated pairs of stocks using the **Engle–Granger test**.  
- Build a **long–short trading strategy** based on the pair’s price spread.  
- Apply a **Z-score based entry/exit rule** to generate trades.  
- Backtest performance with transaction costs, evaluating:  
  - Sharpe ratio  
  - Total return  
  - Number of trades  
  - Win rate  
- Compare **training vs out-of-sample results** to assess robustness.  

---

## 🛠️ Methodology
1. **Data**: Daily adjusted close prices of 12 large-cap US tech stocks (2019–2025).  
2. **Pairs Selection**:  
   - Engle–Granger cointegration test.  
   - Prefiltering to reduce false positives.  
3. **Trading Rules**:  
   - Enter long/short positions when spread Z-score crosses ±2.  
   - Exit when Z-score reverts to 0.  
   - Fixed capital allocation per pair.  
4. **Backtesting**:  
   - Train period: ~70% of data (982 trading days).  
   - Test period: ~30% of data (421 trading days).  
   - Transaction costs included.  
5. **Evaluation Metrics**: Sharpe ratio, returns, win rate, trade frequency.  

---

## 📊 Key Results
- **Total candidate pairs tested**: 66  
- **Top in-sample performers** (Sharpe ratio ranked):  
  - `NVDA–ORCL` (Sharpe ≈ 0.66)  
  - `MSFT–ORCL` (Sharpe ≈ 0.48)  
  - `GOOG–CSCO` (Sharpe ≈ 0.46, Win rate ≈ 78%)  

- **Best out-of-sample pair (showcase)**:  
  - **GOOG–CSCO**  
  - Robust performance with strong mean reversion and high win rate.  

- Detailed plots (spreads, signals, PnL) saved in `project_output/plots/`.  
- Full ranked pair results saved in `project_output/results_pairs_train_vs_oos_with_costs.csv`.  

---

## 🚀 Highlights
- ✅ Automated **pair discovery, ranking, and backtesting pipeline**.  
- ✅ Incorporates **transaction costs** for realistic results.  
- ✅ Identifies **robust trading opportunities** that generalize to out-of-sample data.  
- ✅ Professional, reproducible workflow suitable for **quantitative finance research**.  

---

## 📂 Project Outputs
- `results_pairs_train_ranked.csv` → In-sample ranked pairs.  
- `results_pairs_train_vs_oos_with_costs.csv` → Train vs OOS comparison.  
- `plots/` → Trading signal & performance visualization.  

---

## 🔑 Takeaway
This project demonstrates how to **design, implement, and evaluate a statistical arbitrage (pairs trading) strategy** using cointegration and systematic backtesting.  
It reflects the **workflow and rigor used in professional quant research roles**, bridging **academic modeling** and **real-world trading applications**.  

---


---


## 🙌 About Me

If you're working on financial risk modeling, machine learning, or applied deep learning — let’s connect!

👤 **Surajit Biswas, Ph.D.**  

🔗  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/surajit-biswas-phd/)

📫 surajitbiswas.iiserb@gmail.com

---

## 🏷️ Tags

`Pairs Trading' `Cointegration' `Statistical Arbitrage' `Quant Finance' `Backtesting' `Sharpe Ratio'
