
# Data Science Assignment — Web3 Trading Team

## Candidate
**Anupam Nema**

## Overview
This project analyzes the relationship between **Bitcoin market sentiment** (Fear vs Greed) and **trader performance** using historical trading data from Hyperliquid.

The goal is to uncover patterns in profitability, trading volume, and risk-taking behavior under different sentiment conditions, and to generate actionable insights for smarter trading strategies.

---

## Datasets
1. **Bitcoin Market Sentiment Dataset**
   - Columns: `date`, `value`, `classification` (Fear, Extreme Fear, Greed, Extreme Greed, etc.)
   - Source: Provided Fear & Greed Index CSV.

2. **Historical Trader Data (Hyperliquid)**
   - Columns: `account`, `symbol`, `execution_price`, `size`, `side`, `time`, `start_position`, `event`, `closedPnL`, `leverage`, etc.
   - Source: Provided historical trades CSV.

---

## Methodology
1. **Data Loading & Cleaning**
   - Loaded both datasets and parsed dates.
   - Normalized numeric fields (PnL, leverage, size).
   - Merged datasets on date.

2. **Exploratory Data Analysis (EDA)**
   - Plotted daily total PnL vs sentiment classification.
   - Compared PnL distributions for Fear vs Greed days.
   - Segmented results by leverage buckets, trade sizes, and symbols.

3. **Statistical Testing**
   - Applied t-tests / Mann-Whitney tests to check for significant differences in performance across sentiment regimes.

4. **Segmentation Analysis**
   - Grouped traders by leverage bucket, size bucket, and sentiment to identify segments most sensitive to sentiment changes.

5. **Modeling**
   - Built a baseline model to predict trade profitability using sentiment + trade metadata.

---

## Key Findings
- **Fear Days:** Lower or negative average PnL, suggesting cautious or loss-making behavior.
- **Greed Days:** Higher average PnL, indicating more aggressive and potentially profitable strategies.
- **High-Leverage Trades:** Amplified both gains and losses, with stronger sentiment influence.
- **Smaller Positions:** Less sensitive to sentiment swings.

---

## How to Run
1. Place the trader data CSV in `/mnt/data/trader_data.csv`.
2. Place the Fear/Greed dataset in `/mnt/data/fear_greed.csv`.
3. Open and run the `analysis_notebook.ipynb` file.
4. Review generated plots, statistical summaries, and model results.

---

## Deliverables
- `analysis_notebook.ipynb` — Full code for analysis.
- `slides.pdf` — Summary presentation of findings.
- `README.md` — This documentation file.
- `results_summary.txt` — Email-ready summary.

---


**Anupam Nema**
