# Energy Consumption Prediction

Prediction of energy consumption in the Baltics using regression models and feature engineering.

Main steps of the workflow is:

- Data Wrangling: Changing types, dealing with missing values etc
- Data Analysis: Visualizing the data to find patterns and auto-correlation.
- Feature Generation: Generating features such as date related features and mean/lagged values for features
- Prediction: Predict the consumption for the test data given.
- Prophet is used to forecast the consumption and it is used as a feature in XGBoost. Train a separate prophet model, use the results as features used by the final model (Prophet -> XGBoost + Lags)

