# Time-Series-Project

# Forecasting Microsoft's Stock Price

## A Time-Series Historical Analysis from 1986 to 2023

### Team Members:
- Steven Luo
- Rita Cui
- Serena Zhao
- Amy Sun

---

## Project Overview

In this project, we aim to develop robust forecasting models to predict Microsoft's future stock prices using historical data from 1986 to 2023. By leveraging a comprehensive dataset that includes daily closing prices, high and low prices, and trading volumes, we explore and analyze the stock market trends and patterns associated with Microsoft's performance. Our primary objective is to create accurate forecasting models that can predict future stock prices, providing valuable insights for investors, analysts, and financial enthusiasts.

---

## Agenda

1. Problem Statement
2. Assumptions/Hypotheses
3. Data Properties and EDA
4. Data Processing and Transformations
5. Feature Engineering
6. Proposed Models
7. Results and Future Work

---

## Problem Statement

- Develop robust forecasting models to predict Microsoft’s future stock prices.
- Analyze stock market trends and patterns using historical data from 1986 to 2023.
- Provide accurate forecasts to offer valuable insights for investors and financial analysts.

---

## Assumptions/Hypotheses

- **Stationarity Assumption**: The time series data of Microsoft's stock prices is non-stationary but can be transformed to stationary through differencing or other techniques.
- **Seasonality Hypothesis**: There are seasonal effects in Microsoft's stock prices influenced by factors such as product launches and market conditions.
- **Impact of External Events**: Significant external events (e.g., economic crises, technological breakthroughs, leadership changes) impact Microsoft's stock prices.
- **Correlation between Variables**: A significant correlation exists between stock prices and trading volumes.
- **Modeling Assumption**: A combination of different time series models will provide a comprehensive approach to forecasting.

---

## Data Properties and EDA

- **Summary Statistics**:
  - Mean Closing Price: 48.09
  - Median: 27.09
  - Maximum: 343.11
- **Stationarity Check**:
  - ADF test result indicates the series is non-stationary.
- **Correlation Analysis**:
  - High positive correlations among price-related columns.
  - Moderate correlation between Price and Volume.
- **Visualization**:
  - Time series plots, histograms, and correlation matrices.

---

## Data Processing and Transformations

1. **Anomaly Detection**: Using boxplot method to detect outliers and remove them.
2. **Data Cleaning**: Checking for missing values and applying linear interpolation for imputation.
3. **Stationarity Check**: Applying differencing to make the series stationary and performing ADF test.
4. **Feature Engineering**: Creating lagged features for price and volume.

---

## Proposed Models

1. **ARIMA**: Captures linear dependencies.
2. **SARIMA**: Extends ARIMA to capture seasonality.
3. **Holt-Winters**: Uses exponential smoothing to capture trend and seasonality.
4. **TBATS**: Captures complex seasonal patterns.
5. **ARMA-GARCH**: Combines ARMA for mean and GARCH for volatility modeling.

---

## Model Evaluation

| Model         | RMSE        | MAPE        | MASE       |
|---------------|-------------|-------------|------------|
| ARIMA         | 1.588302    | 1.571954    | 0.998898   |
| SARIMA        | 2.93        | 12.57%      | 0.81       |
| Holt-Winters  | 0.5717961   | 1.533816    | 0.06115833 |
| TBATS         | 0.02833636  | 1.09201     | 0.06286343 |
| ARMA-GARCH    | 1.987949    | 0.01904492  | 1.273061   |

### Key Takeaways
- **TBATS** is the best-performing model, with the lowest RMSE, MAPE, and MASE, indicating superior accuracy and robustness.

---

## Future Directions

1. **Advanced Techniques**: Explore advanced machine learning algorithms such as Random Forest, Gradient Boosting, and Neural Networks for time series forecasting.
2. **Hybrid Modeling Approaches**: Investigate combining the strengths of multiple models (e.g., ARIMA and TBATS, GARCH and TBATS) to capture both linear patterns and complex seasonality.
3. **Incorporation of External Factors**: Use sentiment analysis of news articles, social media, and financial reports to capture market sentiment, which can influence stock prices.

---
