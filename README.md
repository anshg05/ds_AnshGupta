# Trader Behavior Analysis Under Market Sentiment Regimes

## Overview
This project analyzes the relationship between **Bitcoin market sentiment** (Fear & Greed Index) and **trader behavior on the Hyperliquid platform**. The goal is to understand how trader performance, risk exposure, and execution behavior vary across different sentiment regimes and to uncover insights that can support smarter, sentiment-aware trading strategies.

This assignment was completed as part of the **Junior Data Scientist – Trader Behavior Insights** hiring process.

---

## Datasets Used

### 1. Bitcoin Fear & Greed Index
- Provides daily market sentiment labels:
  - Extreme Fear
  - Fear
  - Neutral
  - Greed
  - Extreme Greed
- Used to segment market conditions and analyze behavioral shifts.

### 2. Hyperliquid Historical Trader Data
- Trade-level execution data including:
  - Account identifiers
  - Execution price
  - Trade size (USD)
  - Direction (Buy/Sell)
  - Closed PnL
  - Timestamps

---

## Key Objectives
- Analyze how trader profitability changes under different sentiment regimes
- Study risk-taking behavior (trade size, exposure) during fear vs greed
- Identify behavioral patterns and trader archetypes
- Derive actionable insights for sentiment-aware trading strategies

---

## Project Structure

ds_AnshGupta/
├── notebook_1.ipynb # Complete analysis in Google Colab
├── csv_files/ # Processed datasets
│ ├── merged_sentiment_trades.csv
│ ├── trader_metrics.csv
├── outputs/ # Saved visualizations
│ ├── pnl_by_sentiment.png
│ ├── winrate_by_sentiment.png
│ ├── pnl_boxplot.png
│ ├── trade_size_vs_pnl.png
│ ├── cumulative_pnl.png
├── ds_report.pdf # Final summarized insights & conclusions
└── README.md # Project overview (this file)


---

## Methodology

1. **Data Cleaning & Preparation**
   - Parsed and standardized timestamps
   - Converted trade timestamps from IST to UTC
   - Addressed timezone mismatches between datasets

2. **Dataset Integration**
   - Merged trader data with daily sentiment data using UTC-aligned dates
   - Filtered to sentiment-aligned trades for accurate analysis

3. **Feature Engineering**
   - Created trade-level and trader-level performance metrics
   - Aggregated PnL, win rates, trade volume, and trade sizes

4. **Exploratory Data Analysis**
   - Compared profitability across sentiment regimes
   - Analyzed PnL distributions and risk behavior
   - Visualized trade size vs profitability and cumulative PnL over time

5. **Behavioral Insights**
   - Identified contrarian, momentum, and overconfident trader archetypes
   - Interpreted results using behavioral finance principles

---

## Key Findings

- Market sentiment significantly impacts trader profitability and behavior
- Extreme greed is associated with higher win rates and controlled risk-taking
- Fear regimes show asymmetric payoff opportunities for contrarian traders
- Larger trade sizes do not guarantee higher profitability
- Consistent performance is driven by discipline, not aggressiveness

---

## How to Run the Analysis

1. Open `notebook_1.ipynb` in **Google Colab**
2. Ensure the datasets are available in the working directory
3. Run all cells (`Runtime → Run all`)
4. Processed CSVs will be saved to `csv_files/`
5. Visual outputs will be saved to `outputs/`

---

## Notes
- All analysis was conducted in Google Colab as per instructions
- The notebook is designed to run end-to-end without manual intervention
- Visuals and intermediate data outputs are saved for reproducibility

---

## Author
**Ansh Gupta**  

