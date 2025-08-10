# Data Science Assignment — Web3 Trading Team

**Candidate:** Anupam Nema

## Overview
This project explores the relationship between Bitcoin market sentiment (Fear vs Greed) and trader performance using historical trading data from Hyperliquid.

The analysis covers:
- Data cleaning and preprocessing for both datasets.
- Merging the Bitcoin Fear/Greed Index with trader execution data.
- Exploratory Data Analysis (EDA) and visualization of performance patterns.
- Statistical testing of performance differences between sentiment regimes.
- Actionable insights for trading strategy optimization.

## Files in This Repository

1. **README.md**
   Documentation describing the project, methodology, and files.

2. **avg_pnl_by_sentiment.png**
   Visualization showing the average Closed PnL by market sentiment classification.

3. **ds_report.pdf**
   Final detailed report including methodology, EDA results, statistical findings, and recommendations.

4. **fear_greed_index.csv**
   Dataset containing Bitcoin market sentiment with columns:
   - `date` — Date of observation
   - `value` — Numeric sentiment score
   - `classification` — Sentiment label (Fear, Extreme Fear, Greed, Extreme Greed)

5. **historical_data (1).xlsb**
   Historical trader execution dataset from Hyperliquid with fields:
   - `account` — Trader account ID
   - `symbol` — Asset traded
   - `execution_price`, `size`, `side` — Trade details
   - `closedPnL` — Profit/Loss for the trade
   - `leverage` — Leverage used
   - `time`, `event`, `start_position` — Additional trade metadata

6. **merged_data (2).xlsb**
   Dataset created by merging historical trader data with the sentiment dataset for analysis.

7. **notebook_1[1].ipynb**
   Jupyter notebook implementing the complete analysis workflow:
   - Data loading and cleaning
   - Dataset merging
   - EDA and visualization
   - Statistical testing
   - Segment-level analysis

## How to Run
1. Open `notebook_1[1].ipynb` in Jupyter Notebook, JupyterLab, or VSCode.
2. Place `fear_greed_index.csv` and `historical_data (1).xlsb` in the working directory.
3. Run all notebook cells to reproduce the full analysis and generate the output files.

## Key Findings
- **Fear Days**: Lower average Closed PnL, suggesting more defensive or loss-prone trading behavior.
- **Greed Days**: Higher average Closed PnL, indicating more aggressive and often more profitable trades.
- **Leverage Impact**: High leverage amplifies the sentiment effect — gains in Greed periods, losses in Fear periods.
- **Position Size Effect**: Larger trades tend to be more sensitive to sentiment shifts.

## Author
**Anupam Nema**
