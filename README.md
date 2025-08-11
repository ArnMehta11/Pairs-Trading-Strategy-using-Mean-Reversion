# Pairs-Trading-Strategy-using-Mean-Reversion
Mean reversion trading strategy using z-scores and rolling windows on MSFT &amp; TGT. Features data collection, signal generation, backtesting, and performance analysis to assess the effectiveness of mean reversion in equity trading.

This project implements a mean reversion trading strategy using z-score calculations and rolling windows to identify buy/sell signals on Microsoft (MSFT) and Target (TGT) equities. It explores whether short-term deviations from the mean can be exploited for profitable trading opportunities. Why Target (TGT) and Microsoft (MSFT)? After I added the TGT to my watchlist on my stocks app on the iphone, as I looked at markets everyday I noticed that Target and other consumer-retail companies like Walmart (WMT) move inversely with major technology stocks such as Meta (META), Amazon (AMZN) and Microsoft (MSFT). Knowing that mean-reversion works on MSFT, I implemented this algorithm such that mean reversion  using z-score calculations and rolling windows is applied on MSFT as the "Primary Ticker" and each time the algorithm tells you to go long on MSFT, you allocate half your capital to shorting TGT as the secondary or "pair" ticker.

Features
* Data Collection: Historical price data pulled from Yahoo Finance.
* Signal Generation: Z-score and rolling mean/standard deviation calculations to identify overbought and oversold conditions.
* Backtesting: Simulated trades to evaluate strategy performance over time.
* Performance Analysis: Returns, trade statistics, and equity curves.
8 Visualization: Plots for price, z-score, signals, and cumulative returns.

Methodology
* Rolling Window – Calculate mean and standard deviation of prices over a defined period.
* Z-Score Calculation – Standardize price deviations from the rolling mean.
* Trade Signals: Long Entry: Z-score < -1, Short Entry: Z-score > +1
* Backtesting – Apply signals to historical data and compute strategy metrics.

Notably, as different investors have different risk apetities and may not want to take on any idiosyncratic risk associated with Target or Microsoft, they may download the code and change tickers and use ETFs instead for lower, risk-adjusted returns. 
