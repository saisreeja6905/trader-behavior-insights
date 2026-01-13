# Junior Data Scientist – Trader Behavior Insights

## Assignment Objective
This project was completed as part of the hiring assignment for the **Junior Data Scientist – Trader Behavior Insights** role.  
The objective is to analyze how **Bitcoin market sentiment (Fear & Greed Index)** influences **trader performance and behavior** using historical trading data from Hyperliquid, and to extract insights that can support smarter, sentiment-aware trading strategies.

---

## Datasets
### 1. Bitcoin Market Sentiment (Fear & Greed Index)
- Daily sentiment classification:
  - Extreme Fear
  - Fear
  - Greed
  - Extreme Greed
- Used to capture overall market psychology and emotional regimes.

### 2. Hyperliquid Historical Trader Data
- Trade-level execution data including:
  - Account, coin, execution price
  - Trade size, side (BUY/SELL)
  - Timestamps, fees, closed PnL
- Represents real trader behavior under varying market conditions.

---

## Approach & Methodology
- Cleaned and standardized raw trading data and sentiment data
- Converted timestamps and aligned both datasets at a **daily level**
- Encoded sentiment categories into numeric scores for analysis
- Merged trader performance data with corresponding daily market sentiment
- Engineered key metrics:
  - Average PnL
  - Win rate
  - Trade count
  - PnL distribution
- Visualized trader performance and behavior across sentiment regimes

Robust parsing techniques were used to handle malformed rows and encoding inconsistencies in the raw trading data.

---

## Key Insights
- **Trader performance is strongly influenced by market sentiment**
- Greed and Extreme Greed phases show:
  - Higher average PnL
  - Lower win rates
  - Wider PnL distributions (higher risk and volatility)
- Trade activity increases significantly during Greed phases, indicating **overtrading and elevated risk appetite**
- Fear-driven markets exhibit:
  - More consistent win rates
  - Tighter PnL distributions
  - More disciplined and controlled trading behavior

---

## Implications for Trading Strategy
- Sentiment-aware risk controls can help reduce downside exposure during euphoric markets
- Monitoring trade frequency alongside sentiment can help identify periods of emotional overtrading
- Fear-driven markets may provide better conditions for disciplined or contrarian strategies
- Market sentiment can serve as a valuable behavioral signal alongside price-based indicators

---

## Deliverable
- `01_data_loading_and_overview.ipynb` – Complete analysis notebook with visualizations and insights

---

## Summary
This analysis demonstrates how trader behavior, risk-taking, and performance shift across market sentiment regimes, highlighting the importance of incorporating sentiment signals into trading intelligence and risk management frameworks.
