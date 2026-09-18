# IPL Player Performance Analysis

## Project Overview
This project analyzes IPL player batting performance using statistical data from 2016 to 2025.
The analysis focuses on identifying top performers, understanding relationships between batting metrics, classifying players based on batting style, and building a regression model to predict total runs scored.

## Objective
The main objectives of this project are:
- Analyze player performance based on batting statistics
- Identify top run scorers, six hitters, and consistent performers
- Study relationships between key batting metrics
- Apply regression analysis to predict total runs scored

## Dataset
The dataset contains 500 IPL player records with 21 columns covering batting performance across the 2016–2025 seasons.

The dataset includes information such as:
- Player and team details
- Total runs, matches, and innings
- Highest score and batting average
- Balls faced and strike rate
- Total fours and sixes
- Total fifties and centuries
- Player rankings based on different batting metrics
No missing values were found in the dataset.

## Tools Used
- Python
- Microsoft Excel

## Analysis Performed
- Data understanding and descriptive statistics
- Top run scorer analysis
- Top six hitter analysis
- Consistency analysis
- Fours vs Sixes relationship analysis
- Runs vs Consistency analysis
- Correlation analysis
- Player classification
- Linear regression modelling
- Actual vs Predicted Runs analysis

## Feature Engineering
Two custom features were created during the analysis:
- **Consistency Score** = Total Fifties + Total Centuries
- **Boundary Score** = Total Fours + (2 × Total Sixes)
These features were used to study player consistency and boundary-hitting performance.

## Player Classification

Players were classified into three batting styles based on their boundary distribution:
- **Classical Batsman** — Fours > Sixes
- **Power Hitter** — Sixes > Fours
- **Balanced Player** — Fours = Sixes

## Regression Model
A Linear Regression model was trained using:
- Total Fours
- Total Sixes
- Total Fifties
- Total Centuries
The dataset was divided into 80% training data and 20% test data.

### Model Performance
- **R² Score:** 0.926
- **MAE:** 33.43 runs
- **MSE:** 1739.93
The model showed a strong relationship between the selected batting metrics and total runs scored. :contentReference[oaicite:1]{index=1}

## Key Findings
- Total runs showed a strong relationship with balls faced, fours, consistency, and boundary score.
- Runs vs Balls Faced had a correlation of 0.95.
- Runs vs Total Fours had a correlation of 0.90.
- Runs vs Consistency had a correlation of 0.88.
- Runs vs Boundary Score had a correlation of 0.94.
- Fours and sixes showed a moderate positive relationship with a correlation of 0.45.
- Most players were classified as Classical Batsmen, followed by Power Hitters. :contentReference[oaicite:2]{index=2}

## Repository Contents
- `data/` — IPL dataset used for analysis
- `analysis/` — Python notebook and analysis PDF
- `report/` — Detailed project findings report
