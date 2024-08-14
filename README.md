# 📈 Forecasting COVID-19 Cases in Connecticut with ARIMA Models

## 🎯 Project Overview
This project focuses on using R programming to forecast COVID-19 cases for Connecticut, USA. The aim is to apply ARIMA modeling techniques to provide insights and predictions about the trend of COVID-19 infections

## 📊 Data Overview
The dataset used in this project is titled "2020_Covid_Data.xlsx" and contains time-series data on COVID-19 cases for several US states. Each team member is assigned one US state for analysis.

## 🚀 Deliverables
- **Daily Forecast:** From January 1st, 2021 through February 10th, 2021 for COVID-19 cases in Connecticut

## 🛠️ Technical Approach
- **Modeling:** Fit an `auto.arima(p,d,q) x (P,D,Q)` model to the time-series data of COVID-19 cases for Connecticut.
- **Alternative Models:** Explore and fit alternative ARIMA models as deemed appropriate. Holt-Winters models may also be considered.
- **Model Averaging:** Average the forecasts from the best model and a subset of good models using AICc or BIC weights.
- **Forecast Horizon:** January 1st, 2021 through February 10th, 2021.

## 🧪 What I Have Done
- Loaded and preprocessed the COVID-19 case data for Connecticut.
- Fitted multiple ARIMA models to identify the most suitable model based on information criteria (AICc/BIC).
- Generated and plotted forecasts for the specified period using the best-performing models.

## 📝 Instructions for Running the Project
1. **Load the Data:**
    ```R
    covid_data <- read_excel("path_to/2020_Covid_Data.xlsx")
    ct_data <- covid_data$CT
    ```
2. **Model Fitting:**
    ```R
    library(forecast)
    auto_fit <- auto.arima(ct_data)
    ```
3. **Forecasting:**
    ```R
    forecasted_values <- forecast(auto_fit, h=41)  # Forecasting for 41 days
    plot(forecasted_values)
    ```

## 📚 References
- Data sourced from "2020_Covid_Data.xlsx" available on the course page.
- R Packages: `forecast`, `tseries`, `fpp2`.

## 🤝 Contribution
- This project is part of a collaborative academic exercise. Each team member is responsible for one state, with insights shared across the group.

## 🌟 Key Outcomes
- Developed a robust forecasting model to predict future COVID-19 cases, aiding in better preparedness and response strategies.
- Enhanced understanding of time-series analysis and ARIMA modeling in epidemiological data.

