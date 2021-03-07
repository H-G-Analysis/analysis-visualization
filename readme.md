# Exploration of Ford GoBike data
## by (Hadeer Ismail Gado)


## Dataset

> Ford GoBike data describes individual rides in Bikesharing system all over Francisco Bay area.Tis include information about trip duration,start and end stations information, user type and information about this user for 183412 trip.
>I was interested in the relationship between user_type, gender, age and trip duration. Discovering the most popular station
>Expect that age affects on trip duration and number of trips. Also expect that number of Males user will be greater than females. Most popular station will be affected by most crowded station.
>First, we needed to wrangle the data to explore it correctly:
    >Start_time and end_time columns were string, Converted to date_time format
    >start_station_id and end_station_id were float, converted to int
    >member birthyear was float, converted to int
    >Null values in Station_id, station_name , member birthyear and gender, Null values were dropped.
    >user was born on 1878, replace value with 1978.
    >Filter data with user <=100 years old


## Summary of Findings

>As expected Male users are greater than Female users.
>Number of subscriber is much greater than number of customers.
>As expected younger people who were born between 1980 and 2000 largely exceeds older people
>Trip duration were almost included in one large bin size with long tailed right skewed data, Apply log transformation and foilter data with duration less than or equal 20000 seconds.
>Most Frequent age is Around 30.
>There are nearly 3 frequent spot location in scatter plot for both start and end stations.
>Average trip duration are approximately the same for male, females and others.
>older Females who were born from 1920 to 1949 have slight number of trips, Older males have two apikes in trip duration. others have number of spikes in the middle age.
>Customer trip duration in almost all birthyears was greater than subscribers trip duration


## Key Insights for Presentation

> Added appropriate title for each plot and set location for legend and put title for the legend.