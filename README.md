# Air-Passenger-Demand-Forecast

## Project Overview
The goal of my project is to forecast the U.S. air passenger demand. The source of the data is from https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=259&DB_Short_Name=Air%20Carriers. I chose 23 fields that I would like to analyze on from year 2010 to September 2020, which is the most updated month.

## Exploratory Data Analysis
I did exploratory data analysis to better understand the data by answering six questions, which are
a) In 2019, which airport is the busiest airport for departure?\n 
b) In 2019, which airport is the busiest airport for arrival?\n 
c) From 2010 to 2019 in total, who are the top 5 airlines have most passengers?\ 
d) What is the most passengers change over years among top airlines from 2010 to 2019?\ 
e) Among those top airlines, what is their seat utilization rate like year over year?\ 
f) Among those top airlines, what is their RPK rate over years?

## Forecast

- Model Selection
After I decompose the data, I tried different models, in the end, Arima(0,1,1)(0,1,1)[12] gave me the least AICc values and also only one significant lag in ACF

- Model Comparison
I split the data into training and test. I fit in two models and run the accuracy() function to compare the metrics. Arima(0,1,1)(0,1,1)[12] also gave me the best result.

- Forecast
I use the model I chose to run the forecast for next two years.

