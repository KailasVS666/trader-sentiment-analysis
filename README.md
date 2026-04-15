# Trader Performance vs Market Sentiment Analysis

## Objective
Analyze how market sentiment (Fear vs Greed) impacts trader behavior and performance using Hyperliquid trading data.

---

## Dataset
- Bitcoin Market Sentiment (Fear/Greed Index)
- Historical Trader Data (Hyperliquid)

---

## Methodology

### 1. Data Preparation
- Cleaned and loaded both datasets
- Converted timestamps and aligned data at daily level
- Merged sentiment data with trader activity

### 2. Feature Engineering
- Daily PnL per trader
- Win rate (profitability ratio)
- Trade frequency
- Position type (Long/Short)
- Trader segmentation:
  - Winners vs Losers
  - High vs Low position size

---

## Key Insights

### 1. Trader Performance Varies Strongly by Skill During Greed Phases
Losing traders incur significant losses during Greed conditions, while winning traders remain consistently profitable across all sentiments.

### 2. Fear Conditions Encourage More Stable Trading Behavior
Both winning and losing traders show relatively stable performance during Fear conditions, indicating more cautious trading.

### 3. Position Size is a Major Driver of Profitability
High position size trades generate substantially higher profits across all market conditions, while low-size trades contribute minimal returns.

### 4. Market Sentiment Impacts Weak Traders More
Winning traders remain consistent across conditions, while losing traders are heavily affected by market sentiment.

---

## Tools Used
- Python (Pandas, NumPy)
- Matplotlib, Seaborn
- Jupyter Notebook

---

## How to Run

1. Clone the repository:

    git clone https://github.com/KailasVS666/trader-sentiment-analysis.git

2. Navigate to project folder:

    cd trader-sentiment-analysis

3. Open notebook:

    jupyter notebook notebook/analysis.ipynb

---

## Project Structure

    trader-sentiment-analysis/
    │
    ├── data/
    │   ├── sentiment.csv
    │   └── trades.csv
    │
    ├── notebook/
    │   └── analysis.ipynb
    │
    └── README.md

---

## Summary
This analysis shows that trader performance is influenced not just by market conditions but by behavioral discipline. Overconfidence during Greed phases leads to poor outcomes for weaker traders, while consistent strategies perform well across all conditions.