# Raw-Coal-Prediction-R
Undergraduate Thesis: Time series analysis and forecasting of raw coal production based on R language.
# Time Series Analysis and Forecasting of China's Raw Coal Production

This repository contains the R code and research documentation for my undergraduate thesis in Financial Mathematics. The project analyzes the historical trends of China's raw coal production and implements various statistical models for future forecasting.

##  Project Overview
This study utilizes monthly data of China's raw coal production from **August 2000 to August 2024** (289 observations) sourced from the National Bureau of Statistics. The primary objective is to build robust statistical models to capture the seasonality and trends in energy production.

##  Methodology
The analysis follows a rigorous time series forecasting workflow:
1. **Data Preprocessing**: Logarithmic transformation and seasonal differencing to achieve stationarity.
2. **Exploratory Data Analysis (EDA)**: Decomposition of trend, seasonality, and irregular components.
3. **Statistical Modeling**:
   - **ARIMA Models**: Comparison between `auto.arima()` and manual selection based on ACF/PACF plots and Unit Root Tests.
   - **Seasonal ARIMA**: Identified $ARIMA(1, 0, 1)(0, 1, 1)_{12}$ and $ARIMA(0, 1, 1)(1, 0, 1)_{12}$ as optimal models.
   - **Holt-Winters**: Triple exponential smoothing for additive and multiplicative seasonality.
4. **Forecasting Techniques**: 
   - Residual Bootstrap & Data Bootstrap for ARIMA.
   - Data Bootstrap for Holt-Winters.

##  Key Findings
- The coal production sequence exhibits strong **12-month seasonality** and a clear **upward trend**.
- Combined models successfully predicted production trends for the period from September 2024 to August 2025.
- The study highlights the stability of China's energy output despite seasonal fluctuations.

##  Tech Stack
- **Language**: R
- **Key Libraries**: `forecast`, `tseries`, `ggplot2`, `stats`, `bootstrap`

##  File Structure
- `analysis.Rmd`: The complete R script containing data processing, modeling, and visualization.
- `data.csv`: Raw dataset (CSV) from the National Bureau of Statistics.


## 🎓 About the Author
- **Name**: Youyang Qu
- **Major**: Financial Mathematics


---
*Note: This project is part of an undergraduate thesis and is intended for academic exchange and research purposes only.*
