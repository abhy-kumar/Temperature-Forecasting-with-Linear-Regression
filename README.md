# Temperature Forecasting with Linear Regression

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.3.0-green.svg)
![NumPy](https://img.shields.io/badge/NumPy-1.21.0-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.2-orange.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4.2-red.svg)

## Introduction

This repository contains a Jupyter Notebook that performs temperature forecasting using Linear Regression. By leveraging historical temperature data from 1901 to 2021, the notebook trains separate linear regression models for various temperature metrics, including monthly, seasonal, and annual averages. The models are then used to predict temperatures for the next 20 years. The results are visualized in vertically stacked plots for easy comparison and analysis.

## Features

- **Data Loading & Preprocessing:** Reads temperature data from a CSV file and prepares it for modeling.
- **Multiple Linear Regression Models:** Trains individual models for each temperature metric (e.g., JAN, FEB, ANNUAL).
- **Forecasting:** Predicts temperatures for the next 20 years based on historical trends.
- **Visualization:** Generates clear, vertically stacked plots to compare actual data with forecasted values.
- **Export Predictions:** Saves the forecasted temperatures to a CSV file for further analysis.

## Installation

To run the notebook locally, install Jupyter Notebook and open the .ipynb file in it or just use Google Colab.

## Dataset
The dataset used in this project is assumed to be a CSV file named ``TEMP_ANNUAL_MEAN_1901-2021.csv``, containing historical temperature data with the following columns:

```
YEAR: The year of the recorded temperatures.
JAN, FEB, ..., DEC: Average temperatures for each month.
ANNUAL: Annual average temperature.
JAN-FEB, MAR-MAY, JUN-SEP, OCT-DEC: Seasonal average temperatures.
```
Ensure that the dataset is correctly formatted and placed in the specified directory before running the notebook.

## Visualization
The notebook generates vertically stacked plots for each temperature metric, displaying both actual historical data and forecasted values. This layout facilitates easy comparison of trends across different metrics over the years.

## Predictions
Predicted temperatures for the next 20 years are saved in the ``temperature_forecasts.csv`` file. This CSV includes:

```
YEAR: The forecasted year.
JAN, FEB, ..., DEC: Predicted average temperatures for each month.
ANNUAL: Predicted annual average temperature.
JAN-FEB, MAR-MAY, JUN-SEP, OCT-DEC: Predicted seasonal average temperatures.
```
## License
This project is licensed under the MIT License.
