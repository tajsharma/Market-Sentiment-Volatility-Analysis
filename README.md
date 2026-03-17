# Market Sentiment & Volatility Analysis: An EDA of Financial News 📈

## Overview
In quantitative finance, generating a trading edge requires understanding not just market direction, but the magnitude of market reactions to external catalysts. 

**Core Problem Statement:**
How can we identify the top three most reactive market sectors to specific categories of financial news (measured by trading volume anomalies and price variance) by the end of this analysis, delivering a ranked sensitivity analysis that quantitative analysts can use to optimize volatility-based trading strategies?

## The Issue Tree (Focus Areas)
To keep the exploratory analysis Mutually Exclusive and Collectively Exhaustive (MECE), this project investigates three distinct drivers of market volatility:
1. **Event Category Impact:** How does the *type* of news (Macroeconomic, Corporate, Geopolitical) dictate the volume and price reaction?
2. **Sector Sensitivity:** Which *sectors* (High-Growth, Defensive, Cyclical/Commodity) are inherently the most volatile when exposed to breaking news?
3. **Sentiment Directionality:** How does the *tone* of the news (Strongly Positive, Strongly Negative, Neutral/Mixed) shift the magnitude of the trading volume?

## Data Source
* **Primary Source:** [Financial News Market Events Dataset for NLP 2025](https://www.kaggle.com/datasets/pratyushpuri/financial-news-market-events-dataset-2025) via Kaggle.
* **Size:** 3,024 records | 12 features.
* **Data Profile:** A mixture of NLP-classified categorical data (`Headline`, `Source`, `Market_Event`, `Sentiment`, `Sector`) and hard numerical market metrics (`Index_Change_Percent`, `Trading_Volume`).
* **Data Quality Notes:** The dataset contains an engineered ~5% null rate to simulate real-world data ingestion pipelines, which is systematically handled during the initial cleaning phase.

## Tech Stack
* **Language:** Python 3
* **Data Manipulation:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`
* **Environment:** Jupyter Notebook

## Project Scope
This project is strictly an Exploratory Data Analysis (EDA). The scope involves data cleaning, imputation of missing values, and exploring the statistical relationships between categorical inputs and numerical market outputs. It does *not* include the development of machine learning models or the backtesting of live trading algorithms.

## Repository Structure
.gitignore
README.md
cap2_eda.ipynb          # Main Jupyter Notebook containing the EDA


## How to Run
1. Clone the repository to your local machine.
2. Ensure you have Python installed and create a virtual environment.
3. Install the required dependencies: `pip install pandas numpy matplotlib seaborn jupyter`
4. Launch the notebook: `jupyter notebook`
