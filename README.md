**Web3 Trader Behavior vs Market Sentiment**

**Data Science Assignment – Hyperliquid Trading Team**

**📌 Project Overview**

This project analyzes how trader behavior and performance change under different market sentiment conditions using real trading data from Hyperliquid and the Crypto Fear & Greed Index.

The goal is to understand how Fear, Greed, and Extreme emotions affect:

Profitability

Risk-taking

Win rate

Buy vs Sell strategies

Trader psychology

These insights help Web3 trading firms design sentiment-aware trading strategies.

**Datasets Used**
**1. Hyperliquid Trader Data**

Contains trade-level information such as:

Account ID

Execution price

Trade size (USD & tokens)

Buy / Sell side

Start position

Closed Profit & Loss (PnL)

Each row represents one executed trade.

**2. Crypto Fear & Greed Index**

Provides daily crypto market sentiment:

Extreme Fear

Fear

Neutral

Greed

Extreme Greed

**Data Processing**

The following steps were performed in the Google Colab notebook:

Converted trade timestamps to datetime

Extracted trade dates

Converted sentiment dates

Merged trader data with sentiment data by date

Removed all missing values

Engineered performance and risk features

Performed sentiment-based analysis

**Analyses Performed**

Profitability vs Market Sentiment

Risk Analysis using Trade Size

Win Rate by Sentiment

Buy vs Sell (Long vs Short) Strategy Performance

Behavioral Finance Check (Revenge Trading)

All visualizations are saved in the outputs/ folder.

**Key Findings**

Extreme Greed has the highest profitability and win rate

Fear periods show the highest risk-taking (largest trade sizes)

Selling is more profitable during Greed, while Buying is more profitable during Fear

Traders do not increase trade size after losses → no evidence of revenge trading

**Project Structure**
ds_manisha_ailani/
│
├── notebook_1.ipynb
├── csv_files/
├── outputs/
│   ├── profit_analysis.png
│   ├── risk_analysis.png
│   ├── win_rate.png
│   ├── strategy_analysis.png
│   └── behavior_check.png
├── ds_report.pdf
└── README.md

**Important Note on Data Files**

Due to GitHub file size limits, large CSV files (merged and processed data) are generated dynamically inside the Google Colab notebook and are not stored in this repository.

All data processing and outputs can be reproduced by running the notebook.

**How to Run**

Open notebook_1.ipynb in Google Colab

Upload:

historical_data.csv

fear_greed_index.csv

Run all cells

All results and graphs will be generated automatically

**Author**

Manisha Ailani
M.Sc. Statistics
Central University of Rajasthan
