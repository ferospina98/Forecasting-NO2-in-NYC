# Forecasting Nitrogen Dioxide (NO₂) Levels Across New York City

This project uses time series analysis to model and forecast nitrogen dioxide (NO₂) concentrations across NYC, using historical air quality data.

## Project Overview

- **Goal**: Forecast average NO₂ levels in NYC to evaluate long-term air quality trends.
- **Data**: Aggregated semiannual NO₂ measurements from public datasets.
- **Forecast Horizon**: June 2023 to June 2025.

## Techniques Used

- Data preprocessing and resampling
- Time series decomposition (trend, seasonality, residuals)
- Stationarity testing (ADF & KPSS)
- Forecast modeling using:
  - SARIMA (statsmodels)
  - Prophet (Meta/Facebook)
- Evaluation with MAE and RMSE
- Visualization with Matplotlib and Plotly

## Results

| Model     | MAE  | RMSE |
|-----------|------|------|
| SARIMA    | 9.75 | 9.79 |
| **Prophet** | **0.53** | **0.71** |

Prophet delivered significantly better forecast accuracy, capturing both the long-term trend and semiannual seasonal variation in NO₂ levels.

## How to Run

1. Clone this repo
2. Install dependencies  
   `pip install -r requirements.txt`  
3. Run `notebook.ipynb` or view it on nbviewer.


This project is licensed under the MIT License.
