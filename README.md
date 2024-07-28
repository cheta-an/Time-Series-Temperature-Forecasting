# Time-Series Forecasting of New Delhi's Monthly Temperature

This project demonstrates a time-series forecasting model for predicting the monthly average temperature of New Delhi using historical data.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)

## Introduction
This project utilizes data from the Meteostat API to perform time-series analysis and forecasting on New Delhi's monthly average temperature from January 2000 to January 2024. The model is built using the SARIMAX method from the `statsmodels` library.

## Installation
1. Clone the repository:
   ```
   git clone https://github.com/cheta-an/Time-Series-Forecasting-Temperature.git
   ```
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
## Usage
To run the analysis, use the provided Jupyter notebook in the notebooks directory.
   ```
   jupyter notebook notebooks/code.ipynb
   ```
## Customization
You can customize the forecast by changing the location or the training data period.

1. Modify the latitude and longitude in the code to forecast the temperature for another location. For example, to set the location to London, UK:
   ```
   location = Point(51.5074, -0.1278)
   ```

2. Adjust the start and end datetime values to change the data period. For example, to set the data from January 2010 to December 2020:
   ```
   start = datetime(2010, 1, 1)
   end = datetime(2021, 1, 1)
   ```
## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.