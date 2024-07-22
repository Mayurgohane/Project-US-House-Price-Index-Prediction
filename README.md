# Project-US House Price Index Prediction

# Live demo- https://deployment-using-render-us-home-price.onrender.com

## Summary
This project aims to predict the US House Price Index (HPI) using various economic indicators
from the Federal Reserve Economic Data (FRED) database. The analysis spans from January 2004
to January 2024, employing Ridge and Lasso regression techniques to understand the relationship
between house prices and economic variables. The models demonstrated strong predictive
capabilities, with high R-squared values and low RMSE, indicating their effectiveness in
forecasting house prices. 

## Data Collection
Data was sourced from Federal Reserve Economic Data (FRED) database, covering:
- **House Price Index (CSUSHPISA)**
- **Interest Rates (FEDFUNDS)**
- **Unemployment Rate (UNRATE)**
- **Consumer Price Index (CPIAUCSL)**
- **GDP Growth (A191RL1Q225SBEA)**
- **Population Growth (POPTHM)**
- **Median Income (MEHOINUSA672N)**
- **Consumer Confidence (UMCSENT)**

## Data Preparation
- **Interpolation**: Linear interpolation for missing values.
- **Outlier Removal**: Z-score method for outlier removal.

## Modeling
### Ridge Regression
- **Best Alpha**: 0.01
- **Mean Cross-Validation R²**: 0.9603
- **Test RMSE**: 8.6893
- **Test R²**: 0.9730

### Lasso Regression
- **Best Alpha**: 0.01
- **Mean Cross-Validation R²**: 0.9603
- **Test RMSE**: 8.7070
- **Test R²**: 0.9729

## Key Findings
- **Interest Rates**: Higher rates lower house prices.
- **Unemployment Rate**: Higher unemployment reduces house prices.
- **CPI**: Higher consumer prices increase house prices.
- **GDP Growth**: Higher GDP growth increases house prices.
- **Population Growth**: Negative impact on house prices.
- **Median Income**: Higher income increases house prices.
- **Consumer Confidence**: Higher confidence slightly lowers house prices.

## Conclusion
The Ridge and Lasso regression models demonstrated strong predictive capabilities for the US
House Price Index using selected economic indicators. Both models achieved high R-squared
values and low RMSE values, indicating their effectiveness. The analysis of coefficients provided
insights into the impact of each feature on house prices. The project highlights the importance of
economic indicators in predicting housing market trends and provides a robust framework for
future analyses and model improvements.
