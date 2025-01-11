# Binance-Account-Trade-Analysis

Overview

This project evaluates the performance of various Binance accounts over a 90-day period by analyzing historical trade data and calculating key financial metrics. The project aims to provide actionable insights by ranking accounts based on performance.

Objective

Analyze trade data for 150 Binance accounts.
Calculate financial metrics such as ROI, PnL, Sharpe Ratio, Maximum Drawdown, and Win Rate.
Rank accounts to identify top performers.

Dataset

Source: Binance trade data for 150 accounts.
Key Columns:

Port_IDs: Unique account identifiers.
Trade_History: JSON-formatted trade data (including timestamp, asset, side, and price).

Methodology

Data Cleaning:

Removed missing trade history entries.
Imputed missing values in numeric columns using column means.

Feature Engineering:

Parsed Trade_History to create a detailed dataset for each account.
Created a trade_type column to classify trades (e.g., long_open, long_close).

Metric Calculations:

Return on Investment (ROI): Total realized profit / Total investment.
Profit and Loss (PnL): Total realized profit.
Sharpe Ratio: Risk-adjusted return based on daily profit standard deviation.
Maximum Drawdown (MDD): Largest cumulative returns decline.
Win Rate: Percentage of profitable trades.
Total Positions: Total trades executed.
Ranking Algorithm:
Weighted average of key metrics to rank accounts.

Results

Metrics Calculation:
A comprehensive list of calculated metrics for each account is provided in the calculated_metrics.csv file.

Top 20 Accounts:
A ranked list of the top 20 accounts is available in top_20_accounts.csv.

Key Insights

High ROI and Sharpe Ratio accounts demonstrated consistent, low-risk performance.
High Win Rate and PnL contributed significantly to profitability.
Accounts with substantial drawdowns were ranked lower.

Assumptions

Missing values were imputed with column means.
All trades were treated as independent and equally weighted.
The 90-day period represents typical account performance.

Deliverables

Code: Jupyter Notebook/Python script containing the analysis.
CSV Files:
calculated_metrics.csv: Metrics for all accounts.
top_20_accounts.csv: Ranked list of top 20 accounts.
Report: Detailed explanation of the methodology and findings (Assignment_Report.pdf).
