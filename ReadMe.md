# Predicting Bicycle Traffic

### Tags

Pandas, Visualization,  RollingMean, GroupBy, PivotTable, TimeSeries

### Credits

* [Python Data Science Handbook by Jake Vanderplas](https://amzn.to/2uApdah)  -- Key Source
  * [Section "Example: Visualizing Seattle Bicycle Counts" in Chapter 3](https://www.safaribooksonline.com/library/view/python-data-science/9781491912126/ch03.html#example-visualizing-seattle-bicycle-counts)
  * [Section "Example: Predicting Bicycle Traffic" in Chapter 5](https://www.safaribooksonline.com/library/view/python-data-science/9781491912126/ch05.html#example-predicting-bicycle-traffic)
* [(Blog by Jake Vanderplas) Learning Seattle's Work Habits from Bicycle Counts](https://jakevdp.github.io/blog/2015/07/23/learning-seattles-work-habits-from-bicycle-counts/)



### Objective

Understand Bicylers habits and make predictions



### DataSets Source

* [Seattle Gov - Data](https://data.seattle.gov)
  * [Transportation : Fremont Bridge - Hourly Bicycle Counts by the  month of October 2012 to present](https://data.seattle.gov/Transportation/Fremont-Bridge-Hourly-Bicycle-Counts-by-Month-Octo/65db-xm6k)
    * The Fremont Bridge Bicycle Counter records the number of bikes that cross the bridge using the pedestrian/bicycle pathways. Inductive loops on the east and west pathways count the passing of bicycles regardless of travel direction. The data consists of a date/time field: Date, east pathway count field: Fremont Bridge NB, and west pathway count field: Fremont Bridge SB. The count fields represent the total bicycles detected during the specified one hour period. Direction of travel is not specified, but in general most traffic in the Fremont Bridge NB field is travelling northbound and most traffic in the Fremont Bridge SB field is travelling southbound. 
    * Code: `!curl -o FremontBridge.csv# https://data.seattle.gov/api/views/65db-xm6k/rows.csv?accessType=DOWNLOAD`
* [NOAA - Climate Data Online Search](https://www.ncdc.noaa.gov/cdo-web/search?datasetid=GHCND)
  * While the datasets are free, the way you obtain data from this site is by submitting your email-id and as if you are making an online purchase for free.
  * NOAA makes available their daily [weather station data](http://www.ncdc.noaa.gov/cdo-web/search?datasetid=GHCND) (I used station ID USW00024233) and we can easily use Pandas to join the two data sources. 

### Lessons

* Learn how to play with Time-Series data.