# Quantix Bot Performance Report

| Rank | Bot Name | Live Expected Avg Return (%) | Backtest Expected Avg Return (%) | Live Sharpe Ratio | Backtest Sharpe Ratio | Live Max Drawdown (%) | Backtest Max Drawdown (%) |
|---|---|---|---|---|---|---|---|
| 1 | candle master | 16.61 | 9.13 | 2.5 | 1.63 | -14.8 | -13.87 |
| 2 | candle master | 14.73 | 9.13 | 2.47 | 1.63 | -12.82 | -13.87 |
| 3 | algo link | 13.39 | 12.07 | 2.66 | 1.21 | -15.42 | -38.29 |
| 4 | algo link |  13.39 | 12.07 | 2.66 | 1.21 | -15.42 | -38.29 |
| 5 | Fortune Flow | 6.18 | 15.58 | 1.76 | 2.09 | -12.62 | -16.7 |
| 6 | king damoon  | 5.33 | 7.38 | 5.59 | 2.37 | 0.0 | -10.37 |
| 7 | Gain Master | 4.46 | 2.33 | 2.82 | 0.96 | -4.29 | -16.55 |
| 8 | Ethovate | 7.79 | 0.19 | 0.53 | 0.05 | -13.04 | -20.51 |


## Comparative Analysis

The top three bots, "candle master" (both instances), and "algo link," showcase varying performance characteristics.  Both "candle master" bots exhibit superior live Sharpe and Calmar ratios compared to their backtested results, indicating stronger risk management in live trading despite lower absolute returns.  The difference between live and backtest performance for these bots warrants further investigation.  "algo link" also displays a higher live Sharpe and Calmar ratio, highlighting robust risk-adjusted returns. However, unlike the "candle master" bots, "algo link" shows a higher win rate in backtesting than live performance but a considerably higher profit/loss ratio in live trading, suggesting its live strategy is more effective at identifying high-reward trades, albeit with fewer trades executed.  Ultimately, each bot presents a unique blend of risk and return profiles, highlighting the complexities of algorithmic trading and the challenges in directly translating backtest results to live market outcomes.


## Individual Bot Analysis

### 1. candle master

The crypto bot "candle master" (bot_id: 8e661158-5e93-422e-82cc-7fe23b6960d3) demonstrates a significant disparity between its live and backtest performance.  While the backtest, spanning 1230 days, yielded an impressive 385.1% return despite a 74.74% market increase, the live performance over 235 days resulted in a more modest 117.41% return against a 20.86% market decline.  This difference highlights the challenges of translating backtest results to real-world conditions.  Both live and backtest data show a relatively low win rate (around 49%), but a healthy profit/loss ratio above 1.4, suggesting that winning trades significantly outweigh losing trades.  The bot utilizes a fixed portfolio across ten major cryptocurrency pairs (BTC, BNB, ETH, ADA, TRX, LTC, LINK, DOT, ATOM, SOL), executing a mean of one entry per trade.  Live quarterly reports reveal that while the overall return is positive, profitability varied considerably across quarters, highlighting potential volatility in its strategy. The high Calmar ratios (15.7 live, 4.31 backtest) indicate a reasonable risk-adjusted return, though a substantial worst expected drawdown is noted in both scenarios.


### 2. candle master

The "candle master" bot demonstrates a significant difference between its live and backtest performance.  While the backtest shows a substantial 385.1% return over 1230 days, incorporating 2634 trades with a 45.9% win rate and a profit/loss ratio of 1.40,  live performance reveals a more moderate 58.35% return over 143 days with 247 trades and a 47.4% win rate, resulting in a higher profit/loss ratio of 1.55.  Despite the lower live return, the bot exhibits strong risk-adjusted performance metrics in live trading, boasting a Sharpe Ratio of 2.47 and a Calmar Ratio of 17.21, significantly surpassing its backtest counterparts (Sharpe Ratio 1.63 and Calmar Ratio 4.31). This suggests the bot's live strategy is more robust in managing risk, even if less aggressive in generating returns compared to its backtested potential. The bot trades across a diverse portfolio of 10 crypto pairs and typically holds positions for approximately 19 hours.  Further analysis of the quarterly reports will be needed to understand the reasons for the variance between live and backtest results.


### 3. algo link

The `algo link` bot demonstrates a significant discrepancy between its live and backtest performance. While the backtest shows a substantial 489.3% return over 1100 days, with a considerable number of trades (247), the live performance yielded a more modest 57.51% return over 141 days, involving only 23 trades.  Despite the lower live return, the live bot exhibits a higher Sharpe ratio (2.66 vs 1.21) and Calmar ratio (14.36 vs 2.09), suggesting potentially better risk-adjusted returns in live trading. The live bot's win rate (65.22%) is slightly lower than the backtest (68.02%), but its profit/loss ratio (2.55) is considerably higher than the backtest (1.64). This indicates that while fewer trades were executed live, those trades were more profitable on average.  The bot focuses on the LINK/USDT pair and, based on its 30-day return distribution, has a high probability (73.21%) of generating positive returns in live trading, although the maximum possible return is significantly lower live than in the backtest.  The differences highlight the inherent challenges in translating backtest results into live market conditions.


### 4. Ethovate

Ethovate is a crypto bot trading ETH/USDT that exhibits contrasting performance characteristics between its live and backtest data.  While the backtest, spanning nearly two years (729 days), showed a 7% return despite a significant market change of 180.61%, the live performance over 58 days yielded a more modest 2.54% return against a 46.59% market movement. This discrepancy suggests potential overfitting in the backtest, evidenced by a lower Sharpe Ratio (0.05 vs 0.53) and Calmar Ratio (0.17 vs 1.29) in the backtest compared to live trading.  Live trading shows a higher win rate (63.56% vs 56.03%) and a slightly better profit/loss ratio (1.11 vs 1.03), but also a significantly lower maximum drawdown (-13.04% vs -20.51%). The live bot expectation model predicts a 30-day average return of 7.79%, suggesting that the short live trading period may not fully reflect the bot's potential. The differences highlight the challenges of translating backtested results to real-world market conditions and the need for ongoing monitoring and adjustments.


### 5. Fortune Flow

The Fortune Flow bot (bot_id: `c19e73a7-a1ae-41ad-8049-ae60f9ba7dd8`) demonstrates a notable discrepancy between its live and backtest performance. While the backtest shows a substantial 603.4% return over 1100 days,  the live performance yielded a more modest 24.74% return over 142 days.  Despite this difference, key characteristics remain consistent: a win rate hovering around 55%, a Profit/Loss ratio above 1.4, and Sharpe and Calmar ratios indicating relatively good risk-adjusted returns (1.76 and 6.01 respectively for live, and 2.09 and 5.45 for backtest).  The live bot's 30-day returns distribution suggests a 69% probability of a positive return, with an expected average return of 6.18%.  The bot trades primarily in ETH, BNB, XRP, ADA, LINK, SUI, PEPE, AVAX, and HBAR, executing 245 trades in its live run and significantly more (1839) during backtesting. This difference highlights the challenges of translating backtest results to real-market conditions and suggests a need for further analysis to reconcile the performance gap.


### 6. king damoon 

The crypto bot "king damoon" demonstrates contrasting performance characteristics between its live and backtest runs.  While the live performance shows a modest 8.09% return over 54 days with a remarkably high 100% win rate across only 6 trades, the backtest reveals a significantly higher 37.99% return over 167 days, albeit with a more typical 72.92% win rate from 48 trades. This discrepancy highlights potential overfitting or limitations in the live trading environment. The backtest also experienced a maximum drawdown of -10.37%, unlike the live run's flawless performance.  The live bot's expectation model predicts a high probability (100%) of positive returns within a 30-day period,  while the backtest expectation, based on a much larger dataset, shows a more conservative 73.91% probability of positive returns, hinting at a potentially more realistic assessment of risk. The significantly longer average position duration in the backtest (1 day) compared to the live run (0 days 11:35:00) suggests a difference in trading strategy execution or market conditions.  Further analysis is needed to reconcile the differences and improve live performance to match the backtesting results.


### 7. Gain Master

The Gain Master bot (bot_id: `581d47f7-6b67-48bf-ab10-173869491b75`) demonstrates a strong live performance with a 41.5% return over 295 days, exceeding the market change of 96.55%.  This is achieved with a high win rate (83.08%) and favorable profit/loss ratio (3.53).  However, backtesting data reveals a significantly higher return of 56.27% over 730 days, despite a negative market change (-33.07%), suggesting potential overfitting or market-specific factors influencing live performance.  While the live bot's Sharpe Ratio (2.82) and Calmar Ratio (12.45) indicate robust risk-adjusted returns, these metrics are lower in the backtest (0.96 and 1.51, respectively), highlighting a disparity between simulated and real-world results.  The bot utilizes a live portfolio mode with equal allocation across 10 crypto pairs, executing 201 trades in the live period and 466 in the backtest. The average position duration is relatively short, approximately 14 hours live and 13 hours during backtesting.  Further investigation is needed to reconcile the performance discrepancies and determine the bot's true robustness.


### 8. Band Master

The Band Master bot (bot_id: `ef0286c8-9d93-4c2a-8a4b-a4595b79ac40`) demonstrates a notable contrast between its live and backtest performances.  Live performance over 267 days yielded a substantial 48.99% return, significantly outperforming the market's 53.8% change, with a robust Sharpe ratio of 1.97 and Calmar ratio of 4.44. This strong live performance is characterized by a high win rate (74.83%) and favorable profit/loss ratio (2.27) across 429 trades.  However, backtesting over 730 days showed a more modest 32.62% return, despite a significantly higher number of trades (2036), and considerably lower risk-adjusted metrics (Sharpe ratio 0.43, Calmar ratio 0.5). The discrepancy suggests that Band Master's strategy may be particularly well-suited to the specific market conditions encountered during its live run. Further analysis is needed to identify the key drivers of this performance difference and evaluate its long-term sustainability.


### 9. AdaMooner

The AdaMooner bot demonstrates a significant discrepancy between its live and backtest performance. While the live performance over 104 days yielded a 10.59% return, exceeding the market change of 15.12% by a small margin, the backtest over 1151 days showed a considerably higher return of 876.07%, despite a negative market change of -47.89%.  This suggests potential overfitting in the backtesting model or significant changes in market conditions affecting the bot's live trading strategy.  AdaMooner executes a relatively low number of trades (26 live, 378 backtest), with a consistent win rate above 60% in both live and backtest environments and a favorable profit/loss ratio.  The live bot expectation shows a high probability (80.26%) of positive returns within a 30-day period, although the expected average return is modest (3.66%).  Further investigation is required to reconcile the large disparity between live and backtested results and assess the bot's long-term viability and robustness.


### 10. Motive6

Motive6 demonstrates a significant divergence between its live and backtest performance. While the backtest shows a substantial 270% return over 1100 days,  the live performance, spanning 105 days, yielded a more modest 16.06% return.  Despite this difference, both showcase a consistent positive win rate (64.79% live, 61.04% backtest) and favorable profit/loss ratios (2.06 live, 1.71 backtest).  However, the live bot's Sharpe Ratio (2.85) surpasses its backtested counterpart (1.43), suggesting better risk-adjusted returns in live trading.  The live bot's maximum drawdown (-5.87%) is considerably lower than the backtest (-22.02%), indicating improved resilience to market volatility.  Motive6 trades relatively frequently (71 live trades, 883 backtest trades) with an average position duration around one day. The discrepancy between live and backtest results warrants further investigation, but the live performance metrics, particularly the Sharpe Ratio and maximum drawdown, show promise for this bot's risk-adjusted performance.


