# Nba-Stats-Predictor

## Overview

This project focuses on analyzing NBA players' performances over multiple seasons, specifically comparing historical data with the 2023 NBA season. The goal is to understand trends, evaluate predictive models for player performance (e.g., points scored, rebounds, assists), and ultimately provide insights into the factors influencing player statistics.

## Data Sources

The analysis uses two primary datasets:

- `all_seasons.csv`: Contains historical data of NBA players' performances across various seasons.
- `2023_nba_player_stats.csv`: Provides detailed statistics for NBA players specifically for the 2023 season.

## Methodology

The project employs several steps in data processing and analysis:

1. **Data Preparation**: Initial steps include loading the datasets, identifying common players between the historical and 2023 datasets, and filtering the data accordingly.
2. **Data Cleaning**: Duplicates based on player names are removed to ensure data integrity. Columns are renamed for consistency across datasets.
3. **Exploratory Data Analysis (EDA)**: Descriptive statistics and correlation matrices are generated to understand the data better and identify relationships between variables.
4. **Feature Selection**: Based on the EDA, relevant features are identified for modeling. These typically include Age, Games Played (GP), Points (PTS), Rebounds (REB), and Assists (AST).
5. **Modeling**: Both Linear Regression and Random Forest Regressors are utilized to predict players' performances. The models are evaluated using Mean Squared Error (MSE) and R-squared scores.
6. **Visualization**: Scatter plots are created to visualize the actual versus predicted points, rebounds, and assists, providing a graphical representation of model accuracy.

## Key Findings

- There's a positive correlation between actual and predicted performance metrics, indicating the models capture underlying trends well.
- The models are more reliable in predicting average performances than exceptional ones.
- Random Forest Regressor generally provides a more accurate prediction, as evidenced by lower MSE scores and higher R-squared values compared to Linear Regression.

## Future Work

- **Model Improvement**: Exploring additional features and model tuning could improve prediction accuracy, especially for outlier performances.
- **Comparative Analysis**: Further analysis comparing different seasons or player positions could yield more nuanced insights into performance trends.
- **Deployment**: Developing an interactive tool or application to predict future seasons based on current data trends could be a practical application of this project.

## Conclusion

This project underscores the potential of machine learning techniques in analyzing and predicting sports performances. Through careful data preparation, feature selection, and modeling, it is possible to uncover meaningful insights into NBA player performance trends.
