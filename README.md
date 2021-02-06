# Air-Passenger-Demand-Forecast

## Project Overview
The goal of my project is to forecast the U.S. air passenger demand. The source of the data is from https://www.transtats.bts.gov/DL_SelectFields.asp?Table_ID=259&DB_Short_Name=Air%20Carriers. I chose 23 fields that I would like to analyze on from year 2010 to September 2020, which is the most updated month.

## Exploratory Data Analysis
I did exploratory data analysis to better understand the data by answering six questions, which are<br />
a) In 2019, which airport was the busiest airport for departure?<br />
b) In 2019, which airport was the busiest airport for arrival?<br />
c) From 2010 to 2019, who were the top 5 airlines have most passengers?<br />
d) Which airline changed most over years from 2010 to 2019?<br />
e) Among those top airlines, what was their seat utilization rate like year over year?<br /> 
f) Among those top airlines, what was their RPK rate over years?<br />

## Forecast

- Model Selection

After I decompose the data, I tried different models, in the end, Arima(0,1,1)(0,1,1)[12] gave me the least AICc values and also only one significant lag in ACF

- Model Comparison

I split the data into training and test. I fit in two models and run the accuracy() function to compare the metrics. Arima(0,1,1)(0,1,1)[12] also gave me the best result.

- Forecast

I use the model I chose to run the forecast for next two years.

