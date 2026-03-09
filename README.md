# Predicting Top 50 FIFA Ranked Teams Using Logistic Regression

## Overview
This project analyzes whether a country's football association 
(e.g., UEFA, CONMEBOL, CAF) can predict whether a national team 
belongs to the top 50 in the FIFA world rankings.

Using data from the FIFA rankings before the 2022 World Cup, 
I built a logistic regression model to evaluate how strongly 
regional associations influence the probability of a team being 
ranked in the top 50.

This project demonstrates skills in:
- Data analysis
- Logistic regression modeling
- Statistical inference
- Model evaluation
- Python data science stack

## Dataset
The dataset contains rankings for **211 national teams**, including:

- Team
- Association (AFC, CAF, UEFA, etc.)
- Rank
- Previous Rank
- Points
- Previous Points

Source: FIFA Ranking Data

## Methodology

### 1. Feature Engineering
Created a binary variable:

Top_50 =
1 → Team ranked in top 50  
0 → Team ranked outside top 50

### 2. Model
Logistic Regression:

Top50 = β₀ + β₁ × Association

### 3. Model Evaluation
Metrics used:
- Precision
- Recall
- F1 Score
- Accuracy

Model accuracy: **68%**

### 4. Key Findings
- **UEFA** teams have significantly higher odds of being in the top 50.
- **CONMEBOL** teams also show strong performance.
- **OFC** teams have the lowest probability of appearing in the top 50.

## Technologies Used

- Python
- Pandas
- NumPy
- Statsmodels
- Seaborn
- Matplotlib
- Scikit-learn

## Example Visualization

![Association Ranking](images/association_plot.png)

## Future Improvements

- Add additional predictors such as:
  - GDP per capita
  - Population
  - Domestic league strength
  - Historical performance
- Train more advanced models:
  - Random Forest
  - Gradient Boosting
  - XGBoost

## Author

N'Famara Dabo  
Brown University  
Computer Science & Economics
