# MarketSentimentAnalysis

## Overview

This project explores the relationship between financial news sentiment and the stock price movements of NVIDIA (NVDA). It uses historical opening prices alongside sentiment scores extracted from financial news articles.

All code is provided in Jupyter Notebook format.

## Repository Content

- `Hook.pdf` - Introduces the background and motivation behind this project
- `Rubric.pdf` - Lists deliverables and learning outcomes
- `Granger_causality_Test_Article.pdf` - Provides more details about the Granger causality test and its application [[1]](#1) 
- `How_to_Trade_the_News_Article.pdf` - Discusses how news impacts stock prices and trading strategies [[2]](#2)
- `materials/` folder - Contains notebooks, scripts, data, and instructions needed to reproduce the analysis

## Instructions for Reproducing Results

### 1. Fork the Repository

1. Look for the "Fork" button, usually in the top right corner of the repository page, and click it.

2. You will be prompted to choose which GitHub account to fork the repository to. Select your own account. After forking, you will be redirected to your forked repository page.

### 2. Clone the Forked Repository

- Clone your forked repository:

    `git clone https://github.com/yourusername/your-forked-repo-name.git`

    `cd your-repo-name`

### 3. Create and Activiate a Virtual Environment

- For Mac/Linux:

    `python -m venv venv`

    `source venv/bin/activate`

- For Windows:

    `python -m venv venv`

    `venv\Scripts\activate`

### 4. Install Required Dependencies

- Install all necessary dependencies:

    `pip install requirements.txt`

### 5. Select the Correct Jupyter Kernel

1. Open one of the notebook files

2. Click on "Select Kernel" or "Change Kernel"

3. Choose the kernel that matches your virtual environment, which will be named something like `Python (venv)`

This ensures the notebook runs using the environment with the installed packages.

### 6. Run the Notebooks in Order

Go to the `materials/scripts/` folder and run the notebooks in the order below:

1. `fetch_data.ipynb`
    - Follow the instructions at the top to get your own Alpaca API keys
    - Run the notebook to collect financial news and stock price data from Alpaca API [[3]](#3)[[4]](#4)

2. `get_sentiment.ipynb`
    - This notebook performs sentiment analysis on the news headlines and summaries
    
3. `analysis.ipynb`
    - This notebook performs lag correlation analysis and Granger causality test

#### Notes
- The `analysis.ipynb` notebook contains comments that explain the analytical steps and how to interpret the result

### References

<a id="1">[1]</a> S. Prabhakaran, “Granger Causality Test,” Machine Learning Plus, Aug. 29, 2022. https://www.machinelearningplus.com/time-series/granger-causality-test/ (accessed Apr. 27, 2025).

<a id="2">[2]</a> E. Picardo, “How To Trade The News,” Investopedia. https://www.investopedia.com/articles/active-trading/111313/how-trade-news.asp (accessed Apr. 27, 2025).

<a id="3">[3]</a> “News articles,” Alpaca API Docs, 2025. https://docs.alpaca.markets/reference/news-3 (accessed Apr. 27, 2025).

<a id="4">[4]</a> “Historical bars (single symbol),” Alpaca API Docs, 2025. https://docs.alpaca.markets/reference/stockbarsingle-1 (accessed Apr. 27, 2025).
‌
