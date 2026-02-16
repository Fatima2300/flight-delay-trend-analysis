# Flight Delay Trend Analysis and Forecasting

## Project Overview
This project analyzes historical monthly flight delay data to identify long-term trends and seasonal patterns. Linear regression models are developed to forecast delayed arrivals and evaluate predictive performance.

The analysis demonstrates how time-series modeling and feature engineering can improve forecasting accuracy.

## Dataset
Source: Australian Government – Domestic Airlines On-Time Performance (processed version)
Columns used:
- Month
- Arrivals_Delayed
The dataset contains aggregated monthly flight delay data.

## Objectives
- Analyze delay trends over time  
- Visualize monthly delay patterns  
- Develop a baseline trend model  
- Improve the model using seasonal feature engineering  
- Evaluate performance using R-squared and Mean Absolute Error (MAE)  

## Methods

### 1. Data Preparation
- Converted `Month` to datetime format
- Set month as time-series index
- Sorted data chronologically

### 2. Trend Modeling
- Built a baseline linear regression model using time as predictor
- Identified a statistically significant upward delay trend

### 3. Seasonal Enhancement
- Extracted quarterly seasonality from date index
- Improved model performance (R² increased from 0.153 to 0.187)

### 4. Model Evaluation
- Evaluated statistical significance (p < 0.01)
- Calculated Mean Absolute Error (MAE ≈ 3,974)

## Key Findings
- Flight delays show a statistically significant upward trend.
- Seasonal effects meaningfully influence delay patterns.
- Incorporating seasonality improved explanatory power.
- Predictive accuracy is moderate, suggesting additional variables may enhance performance.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Statsmodels

## Project Structure
- `Flight_Delays_and_Cancellations.ipynb` – Full analysis notebook
- `delayed_arrivals.csv` – Dataset used for analysis

## Conclusion
This project demonstrates practical application of time-series modeling and feature engineering in predictive analytics. Incorporating seasonal patterns improves model performance and provides deeper insight into delay behavior.
