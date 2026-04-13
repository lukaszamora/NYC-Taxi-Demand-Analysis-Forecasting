# NYC-Taxi-Demand-Analysis-Forecasting
This project analyzes NYC yellow taxi trip data to understand demand patterns, congestion behavior, and short-term forecasting. Using three months of trip data, I explore how urban mobility changes over time and evaluate simple models for predicting demand.

![](https://github.com/lukaszamora/NYC-Taxi-Demand-Analysis-Forecasting/blob/main/1%20-%20plot.png)

## Objectives

- Identify temporal patterns in taxi demand  
- Analyze congestion using trip speed  
- Build a baseline and moving average forecasting model  
- Interpret how demand structure affects system behavior  

## Dataset

- [NYC Yellow Taxi Trip Data](https://www.kaggle.com/datasets/marcbrandner/tlc-trip-record-data-yellow-taxi?resource=download&select=yellow_tripdata_2022-08.parquet)  
- Timeframe: August to October 2022  
- Key fields:
  - `pickup_datetime`  
  - `dropoff_datetime`  
  - `trip_distance`  
  - `fare_amount`  

## Data Preparation

- Converted timestamps to datetime format  
- Calculated trip duration in minutes  
- Created time-based features:
  - hour of day  
  - day of week  
  - date  
- Filtered out invalid trips and extreme outliers  

## Exploratory Analysis

### Demand Patterns
- Demand peaks during evening hours  
- Clear weekday vs weekend variation  
- Daily demand shows repeating structure across the dataset  

### Congestion Trends
- Speed decreases during peak demand periods  
- High-demand hours correlate with increased congestion  
- Late-night hours show higher average speeds  

## Time Series Forecasting

### Approach
- Aggregated trips by day  
- Created a time series of daily demand  
- Compared two simple models:
  - naive baseline  
  - moving average  

### Results
- Moving average improved prediction over baseline  
- Forecast captured short-term demand trends  
- Weekly structure visible in smoothed data  

## Key Findings

- Taxi demand follows consistent hourly and weekly patterns  
- Congestion aligns with peak demand periods  
- Short-term demand is predictable using simple models  
- Urban mobility exhibits structured, repeatable behavior over time  

## Tools Used

- Python  
- Pandas  
- Matplotlib  
- Scikit-learn  

## Summary

This project demonstrates how time-based aggregation and simple forecasting techniques can reveal structure in urban transportation systems. The results show that even basic models can provide meaningful insight into demand and congestion patterns.
