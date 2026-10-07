# Store Sales Time-Series Forecasting

## Overview

A machine learning project using historical retail sales data to forecast future store sales. Built as a hands-on project to learn time-series feature engineering, regression, model evaluation, and recursive forecasting.

## Problem Statement

Predict daily sales across multiple stores and product families using historical sales patterns and relevant contextual features.

## Tech Stack

* Python
* Pandas and NumPy
* Scikit-learn
* Kaggle Notebooks

## Approach

* Explored and prepared the retail sales dataset.
* Engineered calendar features, including day of week, month, and weekend indicators.
* Created lag features (7-day and 14-day) and a 7-day rolling mean.
* Incorporated store metadata and oil prices.
* Trained a `HistGradientBoostingRegressor` on log-transformed sales.
* Used recursive forecasting to generate predictions for future dates.

## Results

* Local 16-day recursive validation RMSLE: **0.427638**
* Kaggle public leaderboard RMSLE: **0.62474**
* Kaggle leaderboard rank at the time of submission: **438**

Lower RMSLE indicates better predictive performance. The difference between local validation and leaderboard performance highlighted the importance of realistic validation strategies and forecasting-horizon evaluation.

## Future Improvements

* Improve validation to better match the competition's test horizon.
* Explore additional seasonal and holiday features.
* Compare alternative forecasting models and strategies.

## Dataset

[Store Sales – Time Series Forecasting on Kaggle](https://www.kaggle.com/competitions/store-sales-time-series-forecasting)

*This is a learning project; results reflect the initial baseline model and are not claimed to be state of the art.*
