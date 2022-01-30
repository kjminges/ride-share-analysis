# Module 5 Assignment - PyBer Ride Analysis

## Background
In an attempt to review the differences in the PyBer experience for riders and drivers based on the city type (urban, suburban, and rural), V. Isualize has asked us to distill detailed city (a list of cities where PyBer operates and information regarding the number of drivers and the city type) and rider data (ride data which outlines all rides taken over a ~4 month period, the city they occurred in and the total fare for the ride) into a single dataframe in order to perform the needed analysis. In particular, we were asked to look at the following:

- Ride-sharing summary by city type including the following metrics:
	- Total Rides
	- Total Drivers
	- Total Fares (in USD)
	- Average Fare per Ride
	- Average Fare per Driver
- Total fare by city type over the ~4 month period 

After reviewing the results of the analyses, we then provide recommended actions that the CEO can use to address the disparities between the various city types.

## PyBer Ride Data Analysis
Reviewing the data in more detail, we were able to create the data summary by city type below (see the _PyBer Metrics by City Type_ table). Based on this table, there are many differences in the metrics from one city type to another. It is clear that most rides and drivers are concentrated in the urban cities with 68% of rides taken in the city and 81% of drivers being located in the city. The difference between these two percentages is also telling. When reviewing the number of rides per driver by city type, the variance is massive with rural cities generating 1.6 rides per driver, suburban cities generating 1.3 rides per driver, and urban cities only generating 0.7 rides per driver. These results would suggest that PyBer has not done a good job at matching supply and demand from one city to the next. The urban cities have a supply surplus, while rural cities experience an excess in demand. 

The inefficiencies with supply and demand are most likely driving the discrepancies between the average fares per driver. The increased competition among drivers in urban cities is causing the average fare per driver to be 70% lower than the average fare per driver for rural cities.

As for the average fare per ride, it is difficult to draw too many conclusions given the lack of data used in this analysis. While the average fare per ride in urban cities is 29% lower than rural cities, this may not be driven by the supply of drivers in each location, but by other factors like average length of a ride (time or distance), fees (tolled roads, tickets, etc.), and existence of competition from other ride-sharing companies. Without additional data, it would be irresponsible to draw conclusions from the average fare per ride data. 

When looking at the total fare by city type across a ~4 month span (see the _Total Fare by City Type_ chart), we can see growth in the weekly fares for the urban and suburban city types but given the generally small time period reviewed, it is difficult to determine what is trend vs week-over-week variance. We still believe that this upward trend is something for PyBer to watch in the coming months. If the demand for rides in these two locations is trending up, there may be an argument for softening any of the proposed changes to curb supply in these areas.

In addition to waiting for more time to pass to determine trends for the three city types, it would also be in PyBer's best interest to wait until they have a year's worth of data to look at the seasonality of rides. This will also assist them as they try to review the best way to align supply and demand.

PyBer Metrics by City Type

![PyBer_type_overview](https://github.com/kjminges/PyBer_Analysis/blob/main/analysis/PyBer_type_overview.png)


Total Fare by City Type

![PyBer_fare_summary](https://github.com/kjminges/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

## Conclusion
After reviewing the data and the summaries discussed above, we have the following suggestions for the CEO to try and address the discrepancies that occur between various city types. We believe that the suggestions will allow them to better align supply and demand in both the near term and in the future. 

1. Recruit more riders in rural and suburban cities to increase the supply of drivers to areas with consistent (rural) and growing (suburban cities) demand. This recruitment could also include relocating PyBer drivers from the oversaturated urban cities to the suburban and rural cities. PyPer could offer relocation bonuses and other incentives to facilitate this shift. 
2. If PyBer is unable to get a significant number of drivers in urban cities to move to other locations, PyBer may want to consider letting go of some of their drivers to better align supply and demand. This could be down by dropping the lowest x% of drivers based on average review/rating. 
3. PyBer should continue to monitor trends for a longer time period to assist with their decision making. The current time period provided is too short to pull significant trends from. Once more data is available, they will be able to more accurately differentiate between variance and trend and use this to align the supply of drivers with future demand. 

Before implementing the suggestions, we would suggest PyBer perform a more detailed review of the data including bringing in fields such as ride length, ride distance, as well as a driver dataframe with detailed driver info. 
