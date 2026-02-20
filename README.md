# Trader Behavior Analysis Based on Market Sentiment

## Project Overview

This project analyzes how trader performance changes under different market sentiment regimes (Fear vs Greed).

The objective is to understand behavioral patterns and propose actionable trading strategies.

---

## Dataset Used

1. Historical trade dataset (trade-level PnL, size, timestamps)
2. Fear & Greed Index dataset (daily sentiment classification)

Datasets were merged on trade date.

---

## Methodology

1. Data Cleaning
   - Converted timestamps to datetime format
   - Extracted trade date
   - Standardized sentiment date format
   - Removed missing classifications

2. Feature Engineering
   - Merged trade data with sentiment data
   - Created win/loss indicator
   - Segmented trades by sentiment category

3. Analysis
   - Compared PnL distribution across sentiment regimes
   - Evaluated win rate by sentiment
   - Analyzed trade size and trade frequency
   - Visualized results using boxplots and bar charts

---

## Key Insights

- Extreme Fear periods show higher trade frequency and lower win rate.
- PnL volatility increases during emotionally extreme markets.
- Traders tend to overtrade during Fear regimes.
- Win rate improves during Extreme Greed periods.
- Market sentiment significantly influences trader behavior.

---

## Strategy Recommendations

### 1. Risk Reduction During Extreme Fear
- Reduce leverage by 25–40%.
- Limit maximum trades per day.
- Apply stricter stop-loss rules.

### 2. Controlled Expansion During Extreme Greed
- Allow moderate increase in position size (10–20%).
- Focus on trend-following strategies.
- Maintain disciplined risk controls.

---

## How to Run

1. Clone the repository
2. Install dependencies:  pip install pandas numpy matplotlib seaborn
3. Open Jupyter Notebook and run: Trader_Sentiment_Analysis_YourName.ipynb



---

## Conclusion

The analysis demonstrates that trader behavior is strongly influenced by market sentiment. Incorporating sentiment-aware risk management can improve trading consistency and reduce emotionally driven decision-making.
