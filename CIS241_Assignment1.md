# CIS 241 - Assignment #1: Gender Imbalance in Movie Dialogue Across Film History

## Overview

This project analyzes gender imbalance in movie dialogue across film history using Python in a Jupyter Notebook. By examining how often characters speak—broken down by gender—the analysis uncovers long-term trends in representation and highlights how cultural, social, and industry factors have influenced how films tell stories.

The project combines quantitative analysis with historical interpretation to better understand how gender representation has evolved and where disparities remain.

## Objectives
- Quantify dialogue distribution by gender across movies and decades.
- Identify historical variation in gender representation.
- Compare how dialogue imbalance within genders varies between multiple time periods.
- Explain how pop culture and industry-driven movements impact gender disparities within movies.
__
## Dataset
The dataset contains structured movie dialogue information, including:
- Movie title
- Release year
- Character name
- Character gender
- Number of words spoken (dialogue) 
- Proportion of dialogue per character 
- Duration of the movie in minutes
- Movie Genre based on title
__
## Methodology
1. Data Wrangling & Preparation
- Sorted the dataset by each character’s gender.
- Removed or flagged missing and ambiguous character gender and age entries.
- Changed the data type of the movie’s duration from a nominal variable to a numerical one.
- Aggregated dialogue counts by movie, year, and gender.
2. Exploratory Data Analysis (EDA)
= Calculated total and average dialogue counts by gender
= Examined dialogue share per movie and per decade
- Identified outlier films with extreme gender imbalance
3. Trend Analysis
- Analyzed dialogue distribution per gender across different movie genres and time periods.
- Grouped each movie by the proportion of dialogue spoken by each character and their genders.

## Key Findings
- Male characters consistently receive a larger share of dialogue compared to female characters over a large time period.
- The gender gap slightly decreases in more recent films, but remains substantial.
- The gender of lead characters often accounts for a disproportionate amount of dialogue for each gender.
- Representation improvements are uneven and can vary by genre and time period.

## Discussion: Possible Explanations
The analysis suggests several contributing factors to gender imbalance in movie dialogue:
- Historical dominance of male-centered narratives
- Gender bias in casting, screenwriting, and directing roles
- Industry power structures influencing storytelling decisions
- Cultural norms shaping protagonist selection.
- Slow adoption of inclusive storytelling practices

## Tools & Technologies
- Python
- Jupyter Notebook
- Pandas
- NumPy

## Impact & Applications
This project demonstrates how data science can be applied to cultural and social analysis. Possible implementations might include:
- Media and film studies research.
- Data-driven discussions on representation and equity
- Approval for more comprehensive storytelling in films and entertainment.
