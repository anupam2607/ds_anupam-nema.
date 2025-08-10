Data Science Assignment — Web3 Trading Team
Candidate
Anupam Nema

Overview
This project analyzes the relationship between Bitcoin market sentiment (Fear vs Greed) and trader performance using historical trading data from Hyperliquid.

The workflow includes:

Cleaning and merging the Fear/Greed index with trader execution data.

Performing exploratory data analysis (EDA) and visualizations.

Generating summary statistics and insights to inform trading strategies.

Files in This Repository
1. README.md
This documentation file describing the project, data, and files.

2. avg_pnl_by_sentiment.png
A visualization showing the average Closed PnL for Fear vs Greed periods.

3. ds_report.pdf
Final report summarizing methodology, analysis steps, key findings, and conclusions.

4. fear_greed_index.csv
Bitcoin market sentiment dataset with columns:

date

value (numeric sentiment score)

classification (Fear, Extreme Fear, Greed, Extreme Greed)

5. historical_data (1).xlsb
Historical trader data from Hyperliquid containing:

Account details

Trade metadata (symbol, execution_price, size, side, etc.)

Performance metrics (closedPnL, leverage, etc.)

6. merged_data (2).xlsb
The merged dataset combining trader data with sentiment labels for analysis.

7. notebook_1[1].ipynb
Jupyter notebook containing the full analysis pipeline:

Data loading and cleaning

Merging datasets

EDA and visualization

Statistical testing

Segmentation analysis

How to Run
Open the Jupyter notebook (notebook_1[1].ipynb) in JupyterLab or VSCode.

Ensure the datasets (fear_greed_index.csv and historical_data (1).xlsb) are in the working directory.

Run all cells to reproduce the analysis and visualizations.

Key Findings
Fear Days: Lower average Closed PnL, indicating more cautious or loss-prone behavior.

Greed Days: Higher average Closed PnL, indicating more aggressive and potentially profitable trading.

Leverage levels and position sizes significantly impact the effect of sentiment on performance.

Author
Anupam Nema
