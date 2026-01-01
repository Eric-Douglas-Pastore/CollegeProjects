# CIS 241 - Assignment #2: Correlations between total Team Home Runs and other independent variables (MLB 2023)

## Overview

This project analyzes Major League Baseball (MLB) team-level statistics from the 2023 season to determine which factors are most strongly correlated with the number of runs scored by each team. Using data from the official 2023 MLB Team Stats page, this project aims to answer which offensive, situational, and plate-discipline metrics contribute most to run production across the league.

The project incorporates data exploration, correlation analysis, and hypothesis tests, serving as a foundation for deeper modeling or predictive analytics in baseball performance evaluation.

## Objectives

- Identify which team statistics correlate most strongly with runs scored.
- Compare traditional offensive metrics with advanced indicators.
- Highlight understandings that explain offensive success during the 2023 season.
- Choose 3 independent variables from the data set.
- Create 3 regression plots (these are scatterplots with a regression transform) to compare each independent variable with runs scored.
- Calculate Pearson’s correlation coefficient between each of the independent variables and runs scored.
- Choose two of the three independent variables and run two separate permutation tests, testing the correlation between each independent variable and the number of runs scored.
- Write out the null and alternative hypotheses.
- Run 10,000 permutations using the function we created in class.
- Graph the permutation distribution with a red line showing the observed correlation.
- Calculate a p-value.
- Interpret the plots and the p-value, explaining whether the correlation is statistically significant and/or practically significant.
- Provide a reproducible workflow for sports analytics projects.

## Data Source

- MLB 2023 Team Statistics
- Source: Official MLB team stats page (2023 season)
- Unit of analysis: Team-level season totals

## Key Metrics Analyzed

Variables that have the most notable correlations between runs scored include:

- Batting Average (AVG)
- On-Base Percentage (OBP)
- Slugging Percentage (SLG)
- On-Base Plus Slugging (OPS)
- Hits (H)
- Home Runs (HR)
- Walks (BB)
- Strikeouts (SO)
- Stolen Bases (SB)
- Runs Batted In (RBI)

## Methodology

1. Data Collection
  - Scraped and imported team statistics from the 2023 MLB team stats page.
2. Data Cleaning
  - Merged the Team Batting and Team Pitching CSV files into one Pandas DataFrame
  - Removed non-numeric and redundant variables
3. Exploratory Data Analysis (EDA)
  - Summary statistics
  - Correlation matrices
  - Regression Plots
4. Correlation Analysis
  - Pearson correlation coefficients
  - Ranking variables by strength of relationship to runs scored.
  - Use Hypothesis tests to calculate p-values and determine if the correlations are statistically significant
5. Visualizations
  - Heatmaps
  - Scatter plots for top correlating metrics
  - Histograms for Hypothesis Tests

## Tools & Technologies

- Python
- Pandas
- NumPy
- Altair
- Jupyter Notebook

## Key Findings (Summary)

- On-base metrics (RBI, BA, OBP) show the strongest correlation with runs scored.

---

