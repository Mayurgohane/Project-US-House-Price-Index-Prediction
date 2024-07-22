# Project-US-House-Price-Prediction-2004-2024

#You can view the live demo here- https://deployment-using-render-us-home-price.onrender.com

## Summary
This project predicts the US House Price Index (HPI) using economic indicators from the FRED database (2004-2024). Ridge and Lasso regression models were used, showing high predictive accuracy with R-squared values over 0.97 and RMSE around 8.7.

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
The models effectively predict house prices using economic indicators, providing valuable stakeholder insights.

