# Citi Bike Analytics

## Background

Since 2013, the Citi Bike Program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the [Citi Bike Data](https://www.citibikenyc.com/system-data) webpage.

I was tasked with creating a dashboards and stories to identify some trends/phenomenon in the data.

##  Data

I decided to use the data files from 1/1/2017 through current day (9/1/2022).  There were multiple formats on these files, though, which needed to be updated so the data could be consolidated.

### ETL

In order to get the data in a format that is usable and cleaned up for more accurate dashboards, I used python to do the following:
* Loaded the files from the resources directory with each format in its own dataframe
* Removed unneeded columns from all dataframes
* Renamed the remaining columns so they match across dataframes
* Consolidated the dataframes
* Removed the rows with null values
* Saved the data to a new CSV (including a random sample for a working file during development/testing)

## [Visualizations, Dashboards, Story](https://public.tableau.com/app/profile/kim.price1172/viz/CitiBikeAnalysis_16683868386170/StationMap)


## Map

CitiBike Stations:  As you can see in the map of CitiBike stations the most used stations (larger circles) are closer in to the business areas of NY.  The longer duration trips (color legend), however, tend to start in locations further from the heart of the city.

## Dashbaord: Number of Rides

In diving deeper into the data around the number of trips, you can see trends appearing over the last 5 years.  

There has been an overall increase in the number of trips other than in 2020 and early 2021(coinciding with the COVID Crisis).  

Additionally, the seasonality in the number of rides shows clearing with the higher volumes of rides taking place in the warmer months and peaking around August/September. 

By clicking on a station, you can see that these trends appear consistent across stations.

## Dashboard: Time Duration of Rides

The trip duration trends over time are interesting in that the members' usage appears to remain consistently level, but the causal users have some peaks in warmer months and valleys in colder months.

In general you can see a shift around the time of the COVID crisis to a slightly higher time duration from members.  At this time, the time duration for non riders goes up quite a bit signaling that casual usage has been and continues to be more popular.

##