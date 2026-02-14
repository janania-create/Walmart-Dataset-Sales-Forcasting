# Walmart-Dataset-Sales-Forcasting
This project implements a complete time-series forecasting pipeline using the Walmart Weekly Sales dataset. The objective is to analyze historical sales patterns, capture trend and seasonality, incorporate macroeconomic factors, and generate statistically robust forecasts with uncertainty bounds.
The dataset contains weekly sales data for multiple stores along with external economic indicators including Temperature, Fuel Price, CPI, Unemployment rate, and Holiday Flag. The Date column was converted to datetime format and sales were aggregated at the weekly level across all stores to construct a unified time series.
Exploratory analysis included visualization of overall sales trends and rolling mean smoothing (4-week and 52-week windows) to detect short-term fluctuations and annual seasonality. A time-based 80/20 train-test split was applied to preserve temporal order and avoid data leakage.
Two forecasting approaches were implemented:
1. Exponential Smoothing (Holt-Winters) to model trend and seasonality.
Results were exported as `forecasting_output.csv`, including predicted sales and upper/lower confidence bounds for business interpretation.
This project demonstrates applied time-series modeling, multivariate econometric forecasting, model validation, and uncertainty quantification. It provides actionable insights for demand planning, inventory optimization, and strategic decision-making in retail analytics.
The methodology can be extended with hyperparameter tuning, cross-validation, feature importance analysis, and machine learning-based forecasting models for further performance enhancement.
