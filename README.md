# Walmart-Sales-prediction

## Goal
Estimate the Unit Sales of Walmart retail goods to support their strategic development and plan demand for supply chain.

## Exploratory Data Analysis
- Sales Trend (by state, store, category, department, rolling mean)
- Price Trend (Avg price)
- Calendar distribution

## Feature Engineering
- Evnet related features: event count, post-event, pre-event, type
- Price related fearues: mean, unique items
- Sales related features: lag, rolling mean in different period

## Feature Importance
Get the top 20 important features in three states

## Modeling
Inspired by MLForecast function to faciliate the training process in time series, we used LightGBM to predict sales of 45 stores in 3 states (WI, CA, TX) and did ensembling models to get the final result. First, Train 4 models with different features & store/state. Then, ensembled 4 models to get the new score.

## Result
The private score is 0.56337.
