# ds_Manisha_Ailani
**Web3 Trader Behavior vs Market Sentiment**
**Data Science Assignment – Hyperliquid Trading Analysis**
**Project Overview**

This project analyzes how trader behavior and performance change under different market sentiment conditions using real trading data from Hyperliquid and the Crypto Fear & Greed Index.

The goal is to understand how Fear, Greed, and Extreme market emotions influence:

Profitability

Risk-taking

Win rate

Buy vs Sell strategies

Trader psychology

This helps Web3 trading firms build sentiment-aware trading strategies.

📂 Dataset Description
1. Hyperliquid Trader Data

Contains trade-level information such as:

Account ID

Execution price

Trade size (USD & tokens)

Buy / Sell side

Start position

Closed Profit & Loss (PnL)

Each row represents one executed trade.

2. Fear & Greed Index

Daily crypto market sentiment classified as:

Extreme Fear

Fear

Neutral

Greed

Extreme Greed

🛠 Data Processing Steps

Converted trade timestamps to datetime format

Extracted trade date from each trade

Converted sentiment dates to datetime

Merged both datasets by trade date

Removed all rows with missing values

Created new behavioral and performance features

Grouped trades by market sentiment for analysis

📈 Key Analyses Performed
1️⃣ Profitability Analysis

Compared average PnL across sentiment regimes.

2️⃣ Risk Analysis

Used trade size (USD) as a proxy for risk.

3️⃣ Win Rate Analysis

Calculated percentage of profitable trades per sentiment.

4️⃣ Buy vs Sell Strategy Analysis

Compared profitability of long (BUY) and short (SELL) positions under different sentiments.

5️⃣ Behavioral Finance Check

Analyzed whether traders increase trade size after losses (revenge trading).

🔍 Key Insights

Extreme Greed has the highest profit and win rate.

Fear periods show the highest risk-taking (largest trade sizes).

Selling is more profitable during Greed, while buying is more profitable during Fear.

Traders do not show revenge trading behavior after losses.

These findings show that market emotion strongly drives trading outcomes.

📁 Project Structure
ds_manisha_ailani/
│
├── notebook_1.ipynb          # Complete analysis (Google Colab)
├── csv_files/
│     └── final_merged_data.csv
├── outputs/
│     ├── profit_analysis.png
│     ├── risk_analysis.png
│     ├── win_rate.png
│     ├── strategy_analysis.png
│     └── behavior_check.png
├── ds_report.pdf
└── README.md

▶ How to Run

Open notebook_1.ipynb in Google Colab

Upload:

historical_data.csv

fear_greed_index.csv

Run all cells

Outputs will be generated in the outputs/ folder

💡 Why this matters for Web3 Trading

Understanding how traders behave during Fear and Greed allows trading firms to:

Optimize position sizing

Control risk dynamically

Build emotion-aware trading strategies

Improve profitability and reduce losses

👩‍💻 Author

Manisha Ailani
M.Sc. Statistics, Central University of Rajasthan
Data Science & Web3 Trading Analytics
