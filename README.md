# Uber Trip Demand Forecasting
[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-latest-blue)](https://pandas.pydata.org/)  
[![Plotly](https://img.shields.io/badge/Plotly-latest-orange)](https://plotly.com/python/)  
[![Dash](https://img.shields.io/badge/Dash-latest-purple)](https://dash.plotly.com/)  
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
The Uber Trip Demand Forecasting project provides exploratory data analysis (EDA), visualization, and short-term demand forecasting for Uber trips. It delivers insights into:

- Daily trip patterns and volumes  
- Monthly and weekday trends  
- Weekday vs weekend trip distributions  
- Top dispatching bases by trips and active vehicles  
- Short-term (30-day) forecasting using Prophet, LightGBM, or Gradient Boosting Regressor  
- Peak trip days and forecast summary metrics  

The project is built using Python, Pandas, NumPy, Plotly, Dash, Scikit-learn, and Prophet/LightGBM.

---

## Features
- **Traffic Summary & EDA**: Total trips, average daily trips, active vehicle counts, and top dispatching bases  
- **Forecasting**: 30-day forecast using Prophet (preferred), LightGBM, or Gradient Boosting Regressor  
- **Visualizations**: Time series plots, monthly and weekday bar charts, pie charts, and forecast uncertainty bands  
- **Interactive Dashboard**: Dash dashboard with base-level trip selection and dynamic visualizations  
- **Inline Analysis**: All figures and metrics are presented within the dashboard for immediate insight  

---

## Installation
Clone the repository:

```bash
git clone git@github.com:PanchangniDhangar/uber-trip-demand-forecasting.git
cd uber-trip-demand-forecasting
```
Install dependencies:

```bash
pip install -r requirements.txt
```
## Required Packages
- pandas  
- numpy  
- plotly  
- dash  
- scikit-learn  
- prophet / fbprophet  
- lightgbm (optional, fallback to GradientBoostingRegressor)  

## Usage
Ensure your dataset `Ultimate Merged FOIL.csv` is in the project directory or in one of the following paths:

- `/mnt/data/Ultimate Merged FOIL.csv`  
- `/content/Ultimate Merged FOIL.csv`  
- `/content/drive/MyDrive/Ultimate Merged FOIL.csv`

Run the dashboard:

```bash
jupyter notebook Uber_Trip_Demand_Forecasting.ipynb
```
## Data
`Ultimate Merged FOIL.csv` contains Uber trip data with columns such as:

- `date`: Trip date  
- `trips`: Number of trips per day  
- `active_vehicles`: Number of active vehicles (optional)  
- `dispatching_base_number`: Dispatching base identifier  

The notebook and dashboard handle data cleaning, aggregation, and feature engineering for forecasting.  

## Visualizations
The dashboard produces:

- Total trips per day with 30-day forecast overlay  
- Monthly total trips bar chart  
- Weekday total trips bar chart  
- Weekday vs weekend share pie chart  
- Top 20 bases by trips and active vehicles  
- Base-level time series for selected dispatching base  
- Forecast with uncertainty bands and summary metrics  

All figures are generated interactively within the Dash dashboard.  

## Screenshots
<img width="1920" height="3407" alt="screencapture-127-0-0-1-8050-2025-09-06-00_41_26" src="https://github.com/user-attachments/assets/d119454f-c682-4e05-a25c-fc194f4467d1" />

## License
This project is licensed under the MIT License.  

## Contributing
Contributions are welcome! Please submit pull requests or open issues for bugs, feature requests, or improvements.  

## Contact
For any questions or support, reach out to Panchangni at panchangnidhangar@gmail.com.
