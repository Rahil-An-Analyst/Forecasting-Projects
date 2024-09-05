# Project 2: Forecasting Solar Radiation and Investigating Correlation in Property Prices

## Report
View report here - 
(https://rpubs.com/rahil1998/1216693)


## Overview
This project consists of two tasks aimed at forecasting solar radiation and analyzing the correlation between property prices and population change in Victoria. Task 1 focuses on forecasting solar radiation, while Task 2 investigates the potential spurious correlation between property prices and population change.

### Files
- `Forecasting - Project 2.Rmd`: R Markdown file with code and analysis.
- `project_task1.html`: HTML report of the analysis.
- `data1.csv`, `data2.csv`: Dataset used for forecasting.

## Task 1: Two-Year Ahead Forecasting of Solar Radiation Using Time Series Regression and Exponential Smoothing Models

### Objective
To determine the most accurate and suitable model for forecasting monthly solar radiation two years ahead, using time series regression and exponential smoothing models.

### Data Description
- **Data Source**: Solar radiation and precipitation data.
- **Columns**:
  - Monthly averages of horizontal solar radiation
  - Precipitation
- **Observations**: 660 monthly observations from January 1960 to December 2014.

### Methodology
- **Descriptive Analysis**: Initial analysis to understand the dataset.
- **Model Building**: Evaluated time series regression methods and exponential smoothing models (dLagM package, dynlm package).
- **Best Model**: Holt-Winters’ multiplicative Damped model (Mul.hw.damped) with a MASE measure of 0.2035619.

### Results
- Forecasts for 2015 to 2016 are generated using the Holt-Winters’ multiplicative Damped model.
- The model accurately forecasts solar radiation with detailed plots of observed and forecasted values.

## Task 2: Analyzing the Relationship Between Melbourne Property Price Index and Victoria Population Change

### Objective
To analyze whether the correlation between the quarterly Property Price Index (PPI) in Melbourne and the quarterly population change in Victoria is spurious.

### Data Description
- **Data Source**: Property Price Index and population change data.
- **Columns**:
  - Quarterly Residential Property Price Index (PPI) in Melbourne
  - Quarterly population change over the previous quarter in Victoria
- **Observations**: 54 quarterly observations from September 2003 to December 2016.

### Methodology
- **Correlation Analysis**: Examined the correlation between PPI and population change to determine if it is spurious.

### Results
- Analysis concluded that the correlation between PPI and population change is largely uncorrelated and the observed strong cross-correlations are spurious.

## License
This project is licensed under the MIT License.

## Contact
For more information, please contact [Mohammad Rahil](mailto:smrahil98@gmail.com).
