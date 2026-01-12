# Trader Behavior Insights under Market Sentiment

## Overview
This project analyzes how **trader behavior, performance, and risk exposure** vary under different **market sentiment conditions** (Fear, Extreme Fear, Greed, Extreme Greed) using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.

The goal is to identify **behavioral patterns and hidden signals** that can inform smarter, risk-aware trading strategies in Web3 markets.

---

## Objectives
- Analyze how **profitability, risk, and trading activity** align or diverge from market sentiment  
- Identify **overtrading and emotional risk-taking** behaviors  
- Discover **sentiment-dependent and sentiment-agnostic** trading patterns  
- Translate insights into **actionable trading rules**

---

## Dataset Sources
- **Historical Trader Data (Hyperliquid)**  
  https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view

- **Bitcoin Fear & Greed Index**  
  https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view

---

## Repository Structure
ds_<candidate_name>/
├── assign_1.ipynb # Main analysis notebook (Google Colab)
├── csv_files/ # Generated datasets and metrics
│ ├── baseline_behavior_by_sentiment.csv
│ ├── sentiment_metrics.csv
│ ├── coin_sentiment_performance.csv
│ └── trader_sentiment_performance.csv
├── outputs/ # Saved plots and visualizations
│ ├── pnl_distribution_boxplot.png
│ ├── profit_loss_count_by_sentiment.png
│ ├── coin_sentiment_pnl_heatmap.png
│ └── yearly_pnl_by_sentiment_bar.png
├── ds_report.pdf # Final summarized report
└── README.md


---

## Methodology (High Level)
The analysis is structured into multiple phases:

1. **Data Preparation**
   - Cleaning, deduplication, and date alignment
   - Merging trader data with sentiment data

2. **Baseline Analysis**
   - Trade activity, profitability, risk, and win-rate vs sentiment

3. **Distribution & Risk Analysis**
   - PnL distribution, volatility, fee impact, and overtrading detection

4. **Coin-level Analysis**
   - Sentiment sensitivity and risk concentration per asset

5. **Trader-level Analysis**
   - Consistency, emotional bias, and sentiment dependency

6. **Hidden Pattern Discovery**
   - Risk efficiency, overtrading signals, and sentiment-driven inefficiencies

7. **Strategy Insights**
   - Actionable rules for risk control and smarter trading behavior

---

## Key Findings (Summary)
- Trading activity and risk increase significantly during **Greed**, but profitability does not scale proportionally
- **Fear and Neutral** market conditions show better risk-adjusted performance
- Overtrading and rising fees are major contributors to underperformance
- Larger trade sizes reduce per-trade efficiency
- Consistent traders manage risk independently of sentiment

---

## Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Google Colab (all notebooks are Colab-compatible)

---

## Notes & Assumptions
- Sentiment is treated as a **daily signal** and aligned using trade execution date
- Closed PnL represents realized outcomes only
- Correlation analysis is interpreted as **association, not causation**

---

## Author
Prepared as part of the **Junior Data Scientist – Trader Behavior Insights** assignment.

---

## How to Use
1. Open notebooks using Google Colab  
2. Ensure CSV paths and output directories exist  
3. Run notebooks top to bottom for full reproducibility  

---

## License
This project is for **evaluation and educational purposes only**.
