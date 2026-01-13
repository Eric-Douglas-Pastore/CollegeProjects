# Modeling William Shakespeare with K-Means Clustering
## Overview
This Jupyter Notebook creates a model that clusters all 37 of William Shakespeare's plays to determine which potential groupings of plays might exist. The notebook is designed to reinforce analytical reasoning while demonstrating applied data analysis techniques.

## Purpose
The primary purpose of this notebook is to:
- Analyze relationships between different genres of Shakespearean plays.
- Predict the probability of the 100 most used words in each of Shakespeare’s plays.
- Determine the number of clusters that would produce the most realistic results.
## Structure
### 1. Data refinement and preparation
- Data Cleaning and Wrangling
- Creation of subsets using a vectorizer
- Transformation of a .zip file to a dataset
### 2. Exploratory and comparative analysis
- Assess how many “clusters” are contained in all of Shakespeare’s plays
- Identify patterns within the 100 most common words that appear in Shakespearean plays and how that relates to each cluster.
### 3. Visualizations
- A line chart was used to determine the optimal number of clusters my model should have. Specifically, I utilized the “elbow method,” which involves examining an inertia graph and determining where the “elbow” is located.  That point is then used as the value for the number of clusters.
- A bar graph to visualize the normalized word probabilities across all 37 of William Shakespeare’s plays.
### 4. Interpretation and insight
- This project should be viewed with the impression that the number of clusters in my model represents the total number of genres that writers categorize all 37 of William Shakespeare’s plays.
## Libraries Used
- pandas
- requests
- re
- zipfile
- Altair
- SciKit Learn
  - feature_extraction.text (vectorizer)
  - cluster (KMeans/used to create the model)

## Data Source
https://www.folger.edu/explore/shakespeares-works/download/
## Acknowledgements
- Dr. John R. Ladd
