# Crop Production Prediction in India

## Overview
This project predicts agricultural crop production in India using machine learning regression models, based on historical Crop, Area, and Yield data (2006-2011).

## Problem Statement
India is one of the largest agricultural producers globally, with crop production influenced by area under cultivation and yield per hectare. This project aims to predict crop production using historical patterns, helping in agricultural planning and resource allocation.

## Dataset
* Source: UCT internship dataset
* Original format: Wide format (separate columns per year)
* Reshaped to long format: 240 rows × 5 columns (Crop, Year, Production, Area, Yield)

## Approach
1. Data Cleaning: Removed aggregate/total rows, cleaned column names
2. Data Reshaping: Converted wide-format yearly columns into long format
3. Feature Engineering: Label-encoded Crop and Year
4. Model Training: Linear Regression and Random Forest Regressor
5. Evaluation: RMSE and R² Score

## Results
| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | 14.85 | 0.96 |
| Random Forest | 10.42 | 0.98 |

Random Forest performed best, explaining 98% of the variance in crop production.

## Tech Stack
1. Python
2.Pandas
3.Scikit-learn
4. Matplotlib

## Learnings
*Real-world datasets often require significant reshaping before modeling 
*Random Forest outperformed Linear Regression due to its ability to capture non-linear relationships between Area, Yield, and Production
