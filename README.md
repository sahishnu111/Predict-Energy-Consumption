# Predicting Daily Power Consumption with Machine Learning

This project explores how to use machine learning techniques to predict daily power consumption based on time-based features such as the day of the week, month, and season. The aim is to understand consumption patterns and improve forecasting accuracy — something that can be useful for energy companies, infrastructure planning, and sustainability efforts.

## Project Overview

The dataset used contains daily power usage data with columns like `date`, `power_consumption`, `day_in_week`, `month`, and others. The data was first preprocessed to extract meaningful features, including whether the day was a weekend, what season it fell in, and which part of the month it belonged to.

Three models were trained and evaluated:

- Linear Regression  
- Random Forest  
- XGBoost  

We used standard pipelines for preprocessing — scaling numeric features and one-hot encoding categorical ones. Models were evaluated using RMSE, and their predictions were compared visually with actual values.

## Key Highlights

- Cleaned and transformed raw date columns into useful features.
- Created a pipeline using `ColumnTransformer` and `Pipeline` from scikit-learn.
- Compared three models side by side using RMSE as the main metric.
- Plotted actual vs predicted consumption to evaluate how well the models captured the trend.

## Final Results

- **Best RMSE**: ~399.16 kW  
- **Trend match**: The best model was able to closely follow actual consumption patterns.

## Dataset Info

- Files: `df_train.csv` and `df_test.csv`
- Target column: `power_consumption`
- Date format: daily entries from 2006 onward
- Features include: year, semester, quarter, day of week, day in year, and month

## Tools & Libraries Used

- Python  
- pandas, numpy, matplotlib  
- scikit-learn  
- xgboost  

## Sample Output

A sample plot showing the comparison between actual and predicted power usage is included in the repository.
