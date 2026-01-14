# Modeling William Shakespeare with Neural Networks
## Overview
This Jupyter Notebook is a continued analysis of William Shakespeare’s plays.  Specifically, it aims to create a model using an artificial neural network that can accurately classify all 37 of William Shakespeare's plays by genre. The notebook is designed to reinforce analytical reasoning while demonstrating applied data analysis techniques.
Purpose
## The primary purpose of this notebook is to:
- Continue to analyze relationships between different genres of Shakespearean plays.
- Predict the probability of which genre each Shakespearean play falls under.
- Determine which modifiers in an MLPClassifier would produce the most realistic results.
- Conclude by running multiple simulations to verify the overall model’s reliability.
## Structure
### 1. Data refinement and preparation
- Data Cleaning and Wrangling
- Creation of subsets using a vectorizer
- Creation of a dataset using a variable.
- Transformation of a .zip file to a dataset
### 2. Neural Network Modeling
- Split the Dataframes into training and testing samples with a set seed to ensure repeatability in future runs.
- Use of an MLPClassifier with multiple inputs, including a maximum number of reruns, a logistic function, hidden layers with several neurons, an alpha value to consider outliers, and optimization of weights using “lgbfs”.
- Identify patterns in the neural network’s probabilities in classifying Shakespeare’s plays by genre.
- A results table to show the probabilities of genres that the neural network assumed each play was categorized in.
### 3. Data Validation
- Use of cross-validation steps and a classification report to determine the model’s accuracy in real life.  Specifically, the model’s validity was tested using a classification report, which analyzed accuracy (the percentage of all plays that were correctly classified), precision (the percentage of genres in the test data that were correctly classified), and recall (the percentage of genres in both the training and test data that were correctly classified).  The cross-validation steps were used to determine the overall accuracy and variation of multiple simulations that the neural network could produce.
### 4. Visualization
- A heatmap was used to visualize the confusion matrix, which determines how many plays were correctly sorted by the neural network.  Note that the "romance" row contains only zeros because the model ran into a “divide by zero” error.
### 5. Interpretation and insight
- This project should be viewed with the impression that the model shown is not very accurate when predicting and classifying Shakespearean plays to the correct genre across multiple simulations.

## Libraries Used
- pandas
- requests
- re
- zipfile
- Altair
- SciKit Learn
  - feature_extraction.text (vectorizer)
  - MLPClassifier (Neural Network)
## Data Source
https://www.folger.edu/explore/shakespeares-works/download/
## Acknowledgements
- Dr. John R. Ladd

