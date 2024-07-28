# Time-Series Forecasting of New Delhi's Monthly Temperature

This project demonstrates a time-series forecasting model for predicting the monthly average temperature of New Delhi using historical data.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Introduction
This project utilizes data from the Meteostat API to perform time-series analysis and forecasting on New Delhi's monthly average temperature from January 2000 to January 2024. The model is built using the SARIMAX method from the `statsmodels` library.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/cheta-an/Time-Series-Forecasting-Temperature.git
   cd Time-Series-Forecasting-Temperature
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
## Usage
To run the analysis, use the provided Jupyter notebook in the notebooks directory.
   ```bash
   jupyter notebook notebooks/code.ipynb
   ```
## Customization
You can customize the forecast by changing the location or the training data period:

1. Change Location:
   Modify the latitude and longitude in the code to forecast the temperature for another location. For example, to set the location to London, UK:
   ```bash
   new_location = Point(51.5074, -0.1278)
   data = Monthly(new_location, start, end) 
   data = data.fetch()
   ```

2. Change Training Data Period:
   Adjust the start and end datetime values to change the training data period. For example, to set the training data from January 2010 to December 2020:
   ```bash
   start = datetime(2010, 1, 1)
   end = datetime(2021, 1, 1)
   ```