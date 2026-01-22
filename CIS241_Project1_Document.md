# Tutorials on How to run Hypothesis Tests and Correlation Analysis using Harbor Seals
## Overview
This Jupyter Notebook project demonstrates the creation of hypothesis tests, as well as analysis and visualizations of correlations within datasets.  It explains how to categorize each variable in the dataset using a data dictionary (i.e., is this dataset numeric, categorical, or ordinal, and which subcategory does the data fall under: discrete, continuous, or nominal?).  The notebook accomplishes this by analyzing a dataset relating to aerial photographic surveys of harbour seal populations in California between 2001 and 2003.
## Purpose
The primary purpose of this notebook is to:
- Illustrate the necessary steps for creating a hypothesis test and performing a correlation analysis.
- Explain important concepts relating to hypothesis tests and correlation analysis.
## Structure
### 1. Data Dictionary and Context
- Explanation of where the dataset comes from, as well as how it was collected.
- Categorization of each variable within the dataset.
### 2. Data refinement and preparation
- Data Cleaning and Wrangling
- Creation of multiple columns based on substrates and onshore/offshore location
- Conversion of variables to the correct datatypes
  - TIME_ variable was originally an object, when it should have been of type “time.”
  - DATE_ variable should not include time because it is redundant (i.e., there is already a Time column)
  - Some columns were incorrectly classified as “objects” (AKA strings) when they should have been integers or floats.
### 3. Hypothesis Tests
  Introduction and Explanation of a Hypothesis Test
  Vocabulary terms used in a hypothesis test.
  - Null Hypothesis (H0): A null hypothesis in a statistical test (Denoted as H0 and read as “H-nought”) is the statement that there is no significant correlation between two specified populations, or any observed difference due to random chance.
  - Alternative Hypothesis (H1 or HA): Alternative hypotheses (Denoted as H1 or HA) suggest that there is a significant relationship between two datasets. This represents a researcher’s prediction that they are trying to prove.
  - One-tailed Test: We define H0 as the equality of two values. Our alternative hypothesis suggests that there is only one inequality (value A > value B but not value A < value B, and vice versa).
  - Two-tailed Test: Much like a one-tailed test, we define H0 as an equality of two values. However, our alternative hypothesis suggests that the two values are NOT equal. In other words, the alternative hypothesis cares about both inequalities (value A > value B AND value A < value B).
  - Observed Difference: The difference between the values of two groups that is calculated in our observed sample
  - P-value: The fraction of samples (assuming the null hypothesis is true) that are similar to our observed difference. The letter p denotes it.
  - Significance Level: Often denoted by α (alpha), this represents the probability of rejecting the null hypothesis. Commonly used significance levels include 0.05, indicating a 5% significance.
  - Type I Error: We reject the null Hypothesis when it is actually true.
  - Type II Error: We fail to reject the null hypothesis when it is actually false.
- Example of a hypothesis test that determines if there is a statistically significant difference between aerial photos taken above the shore as opposed to above the water.
- Selection of an appropriate test type for the hypothesis test. (e.g. Comparison of means, correlation between two columns, and Chi-Squared Tests)
- Calculation of observed difference/correlation between two means/variables
- Creation of a permutation function for a comparison of means test.
- Calculation of p-value to determine if the null hypothesis is rejected or not by comparing the p-value to a significance level constant, alpha (usually 0.01, 0.05, or 0.1).
  - The p-value determines the probability of each permutation being as extreme as, or more extreme than, the observed difference/correlation, assuming the null hypothesis is true.
### 4. Correlation Analysis and Visualization
- Introduction and Explanation of Correlation Analysis and Visualization
- Vocabulary terms used in correlation analysis and visualization.
  - Correlation: A statistical measurement that describes the relationship between two or more numerical variables.
  - Correlation coefficient: A number (between -1 and 1) that indicates the strength and direction of a correlation.
  - Positive correlation: When an independent variable increases by one unit, the dependent variable also increases.
  - Negative correlation: When an independent variable increases by one unit, the dependent variable decreases.
  - Bivariate: A type of correlation analysis that determines if a relationship exists between two variables.
  - Multivariate: A type of correlation analysis that determines if a relationship exists between more than two variables.
  - Pearson’s Correlation Coefficient: A coefficient that multiplies the deviations from the mean for two variables and divides by the product of the standard deviations. It is useful for showing the strength of a correlation.
  - Overplotting: Overlapping data points in a scatter plot.
  - Heatmap: A matrix that shows the correlation coefficients between two variables. This is especially useful for multivariate correlation analysis.
- Example of a correlation analysis and visualization project using three variables, PHOTOCOUNT (Number of photographs taken of seal at specific location/time), X (x-position of photograph(s)), and Y (y-position of photograph(s)).
- Creation and Analysis of Scatter Plots to determine if two variables are strongly correlated, as well as a heatmap to determine the correlation coefficients between two variables.
- Explanation of how relevant the correlation analysis and visualizations are to the real world.
### 5. Visualizations
- The hypothesis test tutorial involved a box plot to categorize each photograph by determining whether it was above land, water, or neither, as well as a histogram of the permutations run for the hypothesis test with a vertical line that represents the observed difference in the initial sample.
- The correlation analysis and visualization tutorial used three scatter plots and a heatmap to determine the strength of each correlation coefficient between two out of the three chosen variables.
### 6. Interpretation and insight
This project should be viewed as a guide on how to perform hypothesis tests, correlation analysis, and visualizations.

## Libraries Used
- pandas
- numpy
- altair

## Data Source
https://catalog.data.gov/dataset/harbor-seals-ds106-9df81

## Acknowledgements
Dr. John R. Ladd
