# Data Analysis Report on Autism
## Overview
This Jupyter Notebook is the final project of my CIS 241 (Introduction to Data Science) Class.  
It encompasses concepts that include data wrangling, visualizations, correlation analysis, hypothesis testing, regression models, decision trees, random forests, 
classifier models, confusion matrices, precision, recall, accuracy, and many more.
## Purpose
The primary purpose of this notebook is to:
- Showcase all of the skills that I have acquired during my career at W&J College as a Data Scientist.
- Explain important concepts relating to autism and how the theories involved in Data Science pertain to it.
## Structure
### 1. Introduction
- Explanation of autism and why the dataset was chosen.
  Asking questions that might contribute to and relate to autism.
  1. Does a study’s sample size directly correlate to how many cases were reported?
  2. Will my research show whether the autism diagnosis has increased over the years or not?
  3. Is it possible to predict where a study was conducted? 
  4. Do all countries have the same statistics in terms of autism diagnosis, and if not, why might that be? 
  5. What are the minimum and maximum cutoff ages for correctly diagnosing autism?
  6. If there is a cutoff age, what might it be? 
  7. Can adults be diagnosed with autism and receive treatment? 
  8. Is there a way to predict when a study was/will be published?
### 2. Data Wrangling, Explanation, and Exploration
- Data Cleaning and Wrangling
- Creation of multiple columns based on substrates and onshore/offshore location
- Conversion of variables to the correct datatypes
- Modification of cell values to create consistent formats across columns.
- Renaming columns to better understand what each variable means.
- Determining the average minimum and maximum ages of individuals diagnosed with autism.
- Changes to the scales of each axis in the scatter plot to be logarithmic and more readable.
- Use of a histogram to resolve the question of whether or not the number of autism studies has greatly increased over time.
- A line chart to showcase the change in the number of individuals who were chosen for each study over time.
- Creation of a bar chart to determine which country had the most studies relating to autism, as well as the sample size for each study.
### 3. Hypothesis Testing
-This hypothesis test was conducted to see if there is a statistically significant correlation between a study’s sample size and the number of autistic individuals in each sample.
-Creation of a subset that contains only 2 columns: Sample size and # of reported cases for autistic individuals.
- A modification to the transform_regression function was made to create a line of best fit for a graph with logarithmic scales for both axes.  Specifically, the “method” feature was set to the “pow” option, 
meaning that the “transform_regression()” function creates a logarithmic function.
- Defined the null and alternative hypotheses.
  - Null hypothesis: There is no statistically significant correlation between a study's sample size and the number of autism cases reported in each sample.
  - Alternative hypothesis: There is a statistically significant correlation between a study's sample size and the number of autism cases reported in each sample.
    Specifically, this correlation is positive, meaning that as the sample size increases, so does the number of autism cases reported.
- Creation of a simulation function for a hypothesis test involves correlations between two variables.
- Several permutations of the simulations were run to determine if re-shuffling the data would produce results that are similar to the dataset’s observed correlation.
- Calculation of a p-value to further check if there is a statistically significant correlation between sample size and the number of reported autistic individuals.
### 4. Creating and Interpreting Models
- Creation of multiple regression and classification models using LinearRegression, KNN, decision trees, random forests, and Naive Bayes.
  - The Simple Linear Regression model was used to predict the minimum age at which autism can be accurately diagnosed in individuals.
  - The KNN Regression model was created to determine if there is a limit to an individual’s age before an autism study doesn’t work.
  - The Decision Tree and Random Forest were designed to decide when a study that revolved around autism was conducted.
  - The Naive Bayes model was set up to figure out if a study was performed in the United States, Sweden, or England.
- All four models split the dataset into training and testing portions, each with a preset seed to ensure repeatability for future runs.
- The first model (LinearRegression) requires a test to check for heteroskedasticity, which means that the variance across a model's residuals is inconsistent across different simulations.
- A classification test was run on the Naive Bayes model to figure out how often it correctly classified both the training and test data compared to the actual results.
- After the initial results, cross-validation was performed on each model to find out if the results remained consistent across multiple simulations.
### 5. Visualizations
- Data Exploration:
  - Scatter plots, Bar charts, histograms, line charts, and box plots were used to visualize all the important variables within the dataset.
- Hypothesis Testing:
  - A scatter plot with logarithmic scales for both axes was used to better visualize the correlation between sample size and the # of reported cases.
  - A histogram, along with a vertical red line that is located at the observed correlation’s value, was created to visualize whether the null hypothesis should be rejected.  Specifically, if enough data is to the right of the red line, we fail to reject the null hypothesis.
- Regression and Classification Models
  - Histograms were created for each regression model’s residuals to find out if they (the histograms) were normally distributed, indicating efficient performance among the models.
  - A scatter plot was used to visualize whether the first model had heteroscedasticity.
  - A visual tree was created to figure out the results of the decision tree model, which would determine the most important variables when it comes to predicting which year a study was conducted.
  - The classifier model (Naive Bayes) used a confusion matrix in the form of a heatmap, which was used to visualize how well the model predicted whether or not a study took place in the correct country.
### 6. Interpretation and insight
This project should be viewed as an example of how data scientists conduct tests, as well as the thought process for deciding which predictive models data scientists use.
## Libraries Used
- pandas
- numpy
- altair
- math
- matplotlib
- sklearn (SciKit Learn)
  - train_test_split
  - cross_val_score
  - mean_squared_error
  - r2_score
  - LinearRegression (Model #1)
  - StandardScaler (Model #2)
  - KNeighborsRegressor (Model #2)
  - tree (Model #3)
  - DecisionTreeRegressor (Model #3)
  - plot_tree (Model #3)
  - RandomForestRegressor (Model #3)
  - MultiNomialNB (Naive Bayes)
  - confusion_matrix
classification_report

## Source of Dataset
- https://data.cdc.gov/Public-Health-Surveillance/autism-prevalence-studies/9mw4-6adp/about_data

## Acknowledgements
- Dr. John R. Ladd
