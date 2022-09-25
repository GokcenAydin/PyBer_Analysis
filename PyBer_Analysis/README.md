# PyBer_Analysis

## Overview of the Analysis

The purpose of the Pyber Analysis was to create a summary DataFrame by city type by using Ride Data and City Data 
files as a resource. 
In Deliverable 1, a ride-sharing summary DataFrame per city type was created by getting; 
	* The total rides for each city type,
	* The total drivers for each city type,
	* The total amount of fares for each city type,
	* The average fare per ride for each city type,
	* And the average fare per driver for each city type.
After getting this data, a summary DataFrame was created, cleaned up, it's index was deleted, and formatted.

In Deliverable 2, a multiple-line chart of total fares for each city type was created. After reading the merged 
DataFrame, a new DataFrame with the indices of "city type" and "date" was composed. After resetting the index, a 
pivot table with the specified index, columns and values was composed. Using the loc function, the DataFrame 
was narrowed to specified time interval, and the date was reset to "datetime". Checking the DataFrame 
for datetime usage, another DataFrame was created by using the resample() function by week, and sum of the 
fares for each week was received. 

Finally, using the Matplotlib fivethirtyeight graph style, the resample DataFrame was plotted with df.plot() 
function, and the grap was formatted in accordingly with the instructions. 

## Results

According to the results given in the graph, showing the total weekly of the fares for each type of city, 
Urban areas have given the highest fare values between the specified dates '2019-01-01 - 2019-04-29' with two
peak values of $2500 USD, and an approximate minimum value of $1600 USD.

Suburban areas showed the second highest values after Urban areas with an approximate maximum value of $1400 USD,
and a minimum of $700 USD.

The Rural areas gave the lowest fare values, staying within the 0 to $500 USD scale throughout the specified term.

## Summary

When the DataFrame and graph is evaluated within the given period of time, obviously the Urban area was the most
profitable zone with the highest revenue of fares, and showing two peak values. The lowest fare value in Urban area 
was still higher than the highest fare value of other zones.

Suburban area showed the second highest values, with consideably a stabile movement, except for its peak of 
approximately $1400 USD close to March term.

Rural area showed the most balanced values, staying as the lowest fares of the term, within 0 and $500 USD throughout 
the period, with a single peak of $500 USD in April.

In accordingly with this information, Urban zone might be considered as the highest profitable area compared to Suburban
and Rural areas. 