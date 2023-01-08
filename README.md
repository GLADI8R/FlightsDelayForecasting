# FlightsDelayForecasting

In this project we present a timeseries analysis of flight delays and forecast the future delays using the flight dates, departure delays of particular airlines from 2009-2017.

To start with, we selected SouthWest airline as it has the minimum number of outliers. We then applied the ADF test to get the ADF statistic. Since the p-value and ADF statistic obtained are less than the upperbound conditions, hence we can say that the series is stationary.

From the partial auto-correlation plot, we can see that there is no need for moving average term. Also, the PACF plot shows zero lag drop at lag=5, therefore we can use the arima model for lag of 5.

Next, we fit the ARIMA model for each year from 2009-2017 and predict the results for 2018. 
The root mean square value of predicted and actual value of 2018 data is calculated and found out to be 4.837.
The mean absolute percentage error comes out to be 78%.

Lastly, we have used FBProphet for prediction and finding out the trends weekly, monthly and yearly.
