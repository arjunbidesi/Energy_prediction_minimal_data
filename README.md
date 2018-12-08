# Energy_prediction_minimal_data

A large problem in the energy forecasting industry is the accurate prediction of new buildings’ consumption, without having to use extensive historical data. Our project’s objective is to build an accurate prediction model for energy consumption of buildings starting from the very beginning of their instrumentation.

The data we used to train our predictive model came from Schneider Electric. It tracks 758 buildings over four weeks, identified by Series ID. The data we got for each building is as follows:
Series_ID
Timestamp (hour)
Energy Consumption (watt-hours)
Temperature
(45% NaN)
Surface Area (Categorical)
Inside Base Temperature (Categorical)
Days Off

We had four weeks of hourly data taken for each building: 24 hours ⨉ 7 days ⨉ 4 weeks = 672 samples per building. 

After performing clustering on the staged data, we ran several machine learning algorithms, attaining a highest R^2 score of around 92%. 
The details are in the attached jupyter notebok.

We also have a UI component, that allows users to dynamically witness the changes in consumption patterns on the next week. This can be accessed by running the 'main.py' script.
