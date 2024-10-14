# Basketball HT/FT Bet Analysis Project

This project analyzes the "Half-time/Full-time" (HT/FT) betting type in basketball to assess the potential for developing a profitable long-term betting strategy.

## Project Overview

In this project, we focus on the HT/FT betting type, where the bet is placed on the outcome at half-time and full-time. Specifically, we are interested in two scenarios:
1. The first team leads at half-time but loses the match (HT W1 / FT W2).
2. The first team is trailing at half-time but wins the match (HT W2 / FT W1).

The average odds for each of these outcomes are approximately 8:1. By placing bets on both outcomes in a single game, the combined odds are roughly 4:1. To achieve profitability, more than 25% of these bets must win. Each percentage point above 25% yields an additional profit margin of 1% x 4.

## Project Steps

### Part 1: Data Collection and Visualization
1. **Data Collection:** 
   - We scraped basketball statistics from over 10 seasons using Selenium and processed the data into a usable format for analysis.
2. **Data Visualization:**
   - Visualizations are created to analyze the percentage of profitable games by season, as well as the trends across different stages of the season (preseason, regular season, playoffs).

### Part 2: Machine Learning Model
1. **Model Development:** 
   - We built a machine learning model to predict profitable HT/FT games, utilizing added predictors.
2. **Model Evaluation:** 
   - We tested the effectiveness of the model through backtesting on historical seasons and measured the percentage of profitable games.
3. **Conclusions:**
   - Final analysis results and conclusions are drawn based on the performance of the model.

## Prerequisites

Before running the project, ensure you have the following installed:
- Python 3.7+
- Required libraries: `pandas`, `selenium`, `bs4`, `scikit-learn`, `matplotlib`, `seaborn`.

## Results

The model achieved an average success rate of **0.259%** in predicting profitable HT/FT games.

## Code

- You can find the code for the first part of the project [here](https://github.com/DataM0ney/NBA_Project/blob/main/data_prep.ipynb).
- The code for the second part of the project is available [here](https://github.com/DataM0ney/NBA_Project/blob/main/predictions.ipynb).

## Files Overview

- `data_prep.ipynb` - Notebook for data collection and preparation.
- `predictions.ipynb` - Notebook for model training and predictions.
- `htmls/` - Folder containing scraped HTML pages.
- `dataframes.pkl` - Pickle file with saved dataframes.
