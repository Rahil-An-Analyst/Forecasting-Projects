# Project 3: Time Series Forecasting and Regression Modeling: Mortality, First Flowering Day, and Rank-Based Order Analysis

## Reports
View report here -
(https://rpubs.com/rahil1998/1216696)

## Overview
This project includes three tasks related to time series forecasting and regression modeling. It involves predicting mortality rates, first flowering days, and rank-based order similarity metrics using various regression models and time series techniques.

### Files
- `Assignment 3 - Forecasting.Rmd`: R Markdown file with code and analysis.
- `Forecasting_ Project 3.html`: HTML report of the analysis.
- `mort.csv`, `RBO.csv`, `FFD.csv`, `Covariate x-values for Task 3.csv`, `Covariate x-values for Task 2.csv`: Dataset used for forecasting.

## Task 1: Four-Week Ahead Mortality Forecasting in Paris Using Multiple Predictors

### Objective
To forecast the average weekly mortality in Paris four weeks ahead using multiple predictors and determine the most suitable regression model.

### Data Description
- **Data Source**: Mortality and climate data in Paris.
- **Columns**:
  - Disease-specific averaged weekly mortality
  - Local climate (temperature in Fahrenheit)
  - Size of pollutants
  - Levels of noxious chemical emissions
- **Observations**: 508 weekly observations from 2010 to 2020.

### Methodology
- **Descriptive Analysis**: Initial analysis to understand the dataset.
- **Model Building**: Evaluated various time series regression models (dLagM package, dynlm package).
- **Best Model**: Autoregressive Distributed Lag (ARDL(5,12)) model with all four predictors.

### Results
- Forecasted weekly mortality for the next four weeks.
- Reported point forecasts with confidence intervals.

## Task 2: Univariate Forecasting of First Flowering Day: Four-Year Ahead Predictions

### Objective
To forecast the first flowering day of a plant species four years ahead using univariate time series models.

### Data Description
- **Data Source**: Flowering day and climate data.
- **Columns**:
  - Day of occurrence of the species' first flowering (1-365)
  - Climate factors: rainfall, temperature, radiation, relative humidity
- **Observations**: 31 yearly observations from 1984 to 2014.

### Methodology
- **Descriptive Analysis**: Initial analysis of the dataset.
- **Model Building**: Evaluated univariate time series models (dLagM package, dynlm package).
- **Best Model**: Finite DLM model with Relative Humidity as the regressor.

### Results
- Forecasted first flowering days for the next four years.
- Reported point forecasts with confidence intervals.

## Task 3: Rank-Based Order Similarity Metric and Intervention Analysis

### Task 3 Part (a): Univariate Forecasting of Rank-Based Order Similarity Metric: Three-Year Ahead Predictions

#### Objective
To forecast the annual Rank-based Order similarity metric (RBO) for the next three years using univariate time series models.

#### Data Description
- **Data Source**: Rank-based Order similarity metric and climate data.
- **Columns**:
  - Rank-based Order similarity metric (RBO)
  - Climate factors: rainfall, temperature, radiation, relative humidity
- **Observations**: 31 yearly observations from 1984 to 2014.

#### Methodology
- **Descriptive Analysis**: Initial analysis of the dataset.
- **Model Building**: Evaluated univariate time series models (dLagM package, dynlm package).
- **Best Model**: Autoregressive DLM model (ARDL(12,4)) with Radiation as the regressor.

#### Results
- Forecasted RBO values for the next three years.
- Reported point forecasts with confidence intervals.

### Task 3 Part (b): Intervention Analysis for Rank-Based Flowering Order Similarity Metric: Accounting for the Millennium Drought

#### Objective
To incorporate the impact of the Millennium Drought (1996-2009) into the analysis of the Rank-based flowering Order similarity metric and obtain three-year ahead forecasts.

#### Methodology
- **Intervention Analysis**: Accounted for the Millennium Drought period in the analysis.
- **Best Model**: Dynamic Linear Model (Dyn.model) with significant pulse component at the year 1996.

#### Results
- Reported the impact of the Millennium Drought on the RBO metric.
- Generated three-year ahead forecasts and visualized the results.

## License
This project is licensed under the MIT License.

## Contact
For more information, please contact [Mohammad Rahil](mailto:smrahil98@gmail.com).
