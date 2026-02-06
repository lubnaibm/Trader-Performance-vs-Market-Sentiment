# Trader-Performance-vs-Market-Sentiment
Trader Performance vs Market Sentiment Analysis
(Hyperliquid – Fear & Greed Analysis)
🔹 Methodology:

Data Sources:

Bitcoin Market Sentiment data containing daily sentiment classifications (Extreme Fear → Extreme Greed).

Historical Hyperliquid trader execution data containing account-level trades, timestamps, side (Buy/Sell), and closed PnL.

Data Preparation:

Converted timestamps to daily granularity and aligned both datasets on date.

Merged trader data with sentiment data using a left join on trade date.

Filtered and validated key fields to ensure correct alignment and completeness.

Feature Engineering:

Daily PnL per trader: aggregated closed PnL at account–day level.

Win indicator & win rate: based on positive vs negative trade PnL.

Trade frequency: number of trades per trader per day.

Directional bias (Long/Short ratio): ratio of Buy to Sell trades per day, smoothed to avoid division by zero.

Analysis Approach

Compared performance and behavior metrics across sentiment regimes.

Used boxplots and bar charts to analyze distributions, variability, and behavioral shifts.

Segmented traders based on activity levels (frequent vs infrequent).

🔹 Key Insights
📌 Insight 1: Trader performance varies significantly across sentiment regimes

Boxplots of daily PnL show higher median profitability during Greed and Extreme Greed periods.

Fear and Extreme Fear phases are associated with lower or more volatile returns, indicating challenging market conditions.

📌 Insight 2: Market sentiment strongly influences trader behavior

Trade frequency increases noticeably during Greed and Extreme Greed periods, reflecting higher market participation.

Long/Short ratio analysis shows a clear bullish bias during Greed, while Fear phases exhibit more balanced or defensive positioning.

📌 Insight 3: Frequent traders adapt better to sentiment shifts

Frequent traders tend to outperform infrequent traders, particularly during Greed phases.

Infrequent traders show weaker performance and higher downside exposure during Fear periods.

🔹 Strategy Recommendations:
✅ Strategy 1: Sentiment-aware risk control

During Fear and Extreme Fear periods:

Reduce trading aggressiveness (lower frequency).

Focus on defensive positioning and capital preservation.

During Greed periods:

Allow higher trade activity, but monitor volatility closely.

✅ Strategy 2: Segment-specific execution rules

Frequent traders:

Can capitalize on Greed phases with controlled expansion in trade frequency.

Infrequent traders:

Should avoid overtrading during Extreme sentiment phases and focus on selective, high-conviction trades.

🔹 Conclusion

This analysis demonstrates that market sentiment is closely linked to both trader behavior and performance.
Incorporating sentiment-aware rules into trading strategies can help improve returns while managing risk, particularly during emotionally charged market regimes.
