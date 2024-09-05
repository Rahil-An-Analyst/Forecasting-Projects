# Project 1: Evaluating the Best Regression Model for Forecasting ASX Price Index

## Report
View report here -
(https://rpubs.com/rahil1998/1216686)

## Overview
This project aims to determine the most accurate regression model for forecasting the ASX Price Index using various regressors.

## Objectives
- Identify the best regression model for forecasting the ASX Price Index.
- Perform a descriptive analysis and model-building using Distributed Lag Models.

## Data Description
- **Data Source**: ASX Price Index data.
- **Columns**:
  - ASX All Ordinaries (Ords) Price Index
  - Gold price (AUD)
  - Crude Oil (Brent, USD/bbl)
  - Copper (USD/tonne)
- **Observations**: 161 monthly observations from January 2004 onwards.

## Methodology
- **Descriptive Analysis**: Conducted to understand the data and its distribution.
- **Model Building**: Compared four Distributed Lag Models to identify the best fitting model.
- **Evaluation Metrics**: AIC, BIC, R-squared, and error estimates.

## Results
The best fitting model is the Autoregressive Distributed Lag (ADRL(12,4)) model with an R-squared of 96.17%.

## How to Use
- **Setup**: Requires R and necessary packages (`dLagM`).
- **Usage**: Run `Forecasting  - Project 1.Rmd` in RStudio to generate the analysis report. (Make sure you download and edit the location of ASX_data.csv in the Rmd before running) 

## Files
- `README.md`: This file.
- `Forecasting  - Project 1.Rmd`: The R Markdown file with code and analysis.
- `Forecasting_ Project 1.html`: The HTML report of the analysis.
- `ASX_data.csv`: The dataset used for forecasting.

## License
This project is licensed under the MIT License.

## Contact
For more information, please contact [Mohammad Rahil](mailto:smrahil98@gmail.com).
