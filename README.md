# Household-power-consumption-analysis
Time-series analysis of household electricity consumption

###Project Overview

This project analyzes long-term household electricity consumption using a high-frequency time-series dataset collected at one-minute intervals between December 2006 and November 2010. The dataset contains over 2 million observations and captures key electrical variables such as global active power, reactive power, voltage, current intensity, and appliance-level energy sub-metering.

The aim is to uncover usage patterns, detect trends over time, and understand how different household activities contribute to overall electricity consumption.

###Objectives
1) Handle missing values and prepare data for time-series analysis
2) Explore seasonal, daily, and weekly usage trends
3) Analyze long-term household electricity consumption patterns
4) Generate insights for potential energy efficiency improvements

###Dataset Information
Source: UCI Machine Learning Repository
Available here : (https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set)
The dataset contains 2,075,259 measurements collected over 47 months (Dec 2006 – Nov 2010).

 Features:
date – Date of observation (dd/mm/yyyy)
time – Time of observation (hh:mm:ss)
global_active_power – Total active power consumed (kW)
global_reactive_power – Reactive power (kW)
voltage – Voltage (V)
global_intensity – Current intensity (A)
sub_metering_1 – Kitchen appliances energy usage (Wh)
sub_metering_2 – Laundry room appliances energy usage (Wh)
sub_metering_3 – Water heater & AC energy usage (Wh)

Approximately 1.25% of values are missing due to recording gaps.

###Data Cleaning & Preprocessing
This project includes:

1) Parsing and combining date-time columns into a single timestamp
2) Handling missing values 
3) Converting data types for memory optimization
4) Creating time-based features (hour, day, month, year)
5) Resampling data for different time granularities (hourly, daily, monthly)

###Exploratory Data Analysis (EDA)

Key analyses performed:
1) Distribution of global active power consumption
2) Time-series decomposition (trend, seasonality, residuals)
3) Daily and seasonal consumption patterns
4) Correlation between electrical variables
5) Appliance-level energy usage comparison
5) Peak usage time identification

###Key Findings
1) Electricity consumption follows distinct daily and weekly behavioral patterns.
2) Demand is highest during weekends and evening hours.
3) Two major consumption states exist: low-activity and high-activity periods.
4) Seasonal trends suggest changing energy needs throughout the year.
5) Occasional high-consumption spikes occur but appear to be part of normal household behavior.
6) Overall demand patterns are stable enough for reliable forecasting.

###Tools & Technologies
Python (Pandas,NumPy,Matplotlib,Statsmodels-for time-series decomposition)
Jupyter Notebook

###Future Improvements
1) Apply forecasting models (ARIMA, Prophet, LSTM).
2) Detect anomalies in energy consumption.
3) Build an interactive dashboard (Plotly Dash / Power BI).
