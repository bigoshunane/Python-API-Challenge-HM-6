# Python_API_Challenge_HM6

The aim of this project is to develop Pyhton Script which can visualize:
1. The weather of 500+ cities across the world of varying distance from the equator.
2. Plan future vacations based on this weather data anaysis.
To accomplish this, a [simple Python library][https://pypi.org/project/citipy/] and the [OpenWeatherMap API][https://openweathermap.org/api] are used to create a representative model of weather across world cities.

# Part.I  WeatherPy

Final repoert summary covers the following points:

1. Build a series of scatter plots to showcase the following relationships:

       . Temperature (F) vs. Latitude
       . Humidity (%) vs. Latitude
       . Cloudiness (%) vs. Latitude
       . Wind Speed (mph) vs. Latitude
       
2. Run linear regression on each relationship, only this time separating them into Northern Hemisphere greater than or equal to 0 degrees latitude) and Southern      Hemisphere (less than 0 degrees latitude):

       . Northern Hemisphere - Temperature (F) vs. Latitude
       . Southern Hemisphere - Temperature (F) vs. Latitude
       . Northern Hemisphere - Humidity (%) vs. Latitude
       . Southern Hemisphere - Humidity (%) vs. Latitude
       . Northern Hemisphere - Cloudiness (%) vs. Latitude
       . Southern Hemisphere - Cloudiness (%) vs. Latitude
       . Northern Hemisphere - Wind Speed (mph) vs. Latitude
       . Southern Hemisphere - Wind Speed (mph) vs. Latitude
      

Final notebook includes:

     . Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
     . Perform a weather check on each of the cities using a series of successive API calls.
     . Include a print log of each city as it's being processed with the city number and city name.
     . Save a CSV of all retrieved data and a PNG image for each scatter plot.

# Part.II VacationPy

Report includes:

1.Create a heat map that displays the humidity for every city generated from Part.I WeatherPy.

2.Narrow down the DataFrame to find your ideal weather condition, by intruducing the following parameters:

    . A max temperature lower than 90 degrees but higher than 70.
    . Wind speed less than 10 mph.
    . Zero cloudiness.
    
# Final observations summary


    
    
