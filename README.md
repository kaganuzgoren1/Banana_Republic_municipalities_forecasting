# Banana_Republic_municipalities_forecasting
TASK: Forecasting bus demand in Banana Republic municipalities.

The central urban planning committee of Banana Republic asked you to help them forecast municipalities' bus demands. And they provide a nice dataset to support you (https://pi.works/3w8IJbV). The dataset includes two measurements for an hour for the number of used buses in each municipality; each measurement is timestamped. There are 10 municipalities (ids from 0 to 9) and two measurements for an hour. It is aimed to forecast the hourly bus usage for next week for each municipality. The last two weeks (starting from 2017-08-05 to 2017-08-19) are used as assessment (test) data. 

1st step of the project is to aggregate the two measurements for each hour by taking the maximum value. This means that I look at the two measurements for each hour and take the higher of the two as the final value. I did this using pandas' groupby() and max() functions.

2nd step of the project is to model the data with a time series model. This means that I choose a model that can capture the temporal dependencies in the data and make predictions for future time steps.

For the project, 3 different forecasting methods are used. 1st is the Sckit-learn linear regression, 2nd is the XGBoost, and the 3rd is the CNN with Keras. The mean absolute error for each model is written after their implementation for forecasting. 
