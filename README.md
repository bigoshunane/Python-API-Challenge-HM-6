# Python_API_Challenge_HM6

The aim of this project is to develop Pyhton Script which can visualize:
1. The weather of 500+ cities across the world of varying distance from the equator.
2. Plan future vacations based on this weather data anaysis.
To accomplish this, a [simple Python library](https://pypi.org/project/citipy/) and the [OpenWeatherMap API](https://openweathermap.org/api) are used to create a representative model of weather across cities in the world.

Python script developed ,cities data and figures are in the repository under file names Images, WeatherPy and VacationPy and output_data.

# Part.I  WeatherPy

Final repoert summary covers the following points:

1. Build a series of scatter plots to showcase the following relationships:

       . Temperature (F) vs Latitude
       . Humidity (%) vs Latitude
       . Cloudiness (%) vs Latitude
       . Wind Speed (mph) vs Latitude
       
2. Run linear regression on each relationship, only this time separating them into Northern Hemisphere greater than or equal to 0 degrees latitude) and Southern      Hemisphere (less than 0 degrees latitude):

       . Northern Hemisphere - Temperature (F) vs Latitude
       . Southern Hemisphere - Temperature (F) vs Latitude
       . Northern Hemisphere - Humidity (%) vs Latitude
       . Southern Hemisphere - Humidity (%) vs Latitude
       . Northern Hemisphere - Cloudiness (%) vs Latitude
       . Southern Hemisphere - Cloudiness (%) vs Latitude
       . Northern Hemisphere - Wind Speed (mph) vs Latitude
       . Southern Hemisphere - Wind Speed (mph) vs Latitude
      

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

Reoprts:

Temperature (F) vs Latitude

![tvl](https://user-images.githubusercontent.com/84547558/152062547-5444d87e-e639-4129-aa0c-23c050f539f6.png)

    
 Humidity (%) vs Latitude
 
![hvl](https://user-images.githubusercontent.com/84547558/152062807-af960fe0-6074-42ce-bf31-26347c1b5074.png)

Cloudiness (%) vs Latitude

![cvl](https://user-images.githubusercontent.com/84547558/152062943-621ebb4a-144c-4829-aea1-64e44c01a2aa.png)

Wind Speed (mph) vs Latitude

![wvl](https://user-images.githubusercontent.com/84547558/152063035-8b00ee76-400b-4861-b7cb-73efc11b1871.png)

 Northern Hemisphere - Temperature (F) vs Latitude
 
 ![tvln](https://user-images.githubusercontent.com/84547558/152063154-86fff225-c514-417c-96d9-e305ef486d3c.png)

 Southern Hemisphere - Temperature (F) vs Latitude
 
 ![tvlsh](https://user-images.githubusercontent.com/84547558/152063246-331018cc-d22c-40d5-a8d8-9d9607e82514.png)

 Northern Hemisphere - Humidity (%) vs Latitude
 
![hlpn](https://user-images.githubusercontent.com/84547558/152063410-1d10f73e-83b1-4e17-8119-2c0f3ba48e5f.png)

 Southern Hemisphere - Humidity (%) vs Latitude
 
 ![hlshh](https://user-images.githubusercontent.com/84547558/152063527-a76b8fc7-a9ab-47fd-b6f3-2e51e0f0297d.png)

 Northern Hemisphere - Cloudiness (%) vs Latitude
 
 ![cn](https://user-images.githubusercontent.com/84547558/152063656-e6f553a4-ee13-4bf6-a66b-7441786a408f.png)
 
 Southern Hemisphere - Cloudiness (%) vs Latitude
 
![shcc](https://user-images.githubusercontent.com/84547558/152063865-80dc4aaa-d21c-40d5-adbf-600ebdfd810d.png)

 Northern Hemisphere - Wind Speed (mph) vs Latitude
 
 ![wns](https://user-images.githubusercontent.com/84547558/152064022-49ed22e4-aebd-42e1-9e91-13f19aec9ec7.png)
 
 Southern Hemisphere - Wind Speed (mph) vs Latitude
 
![hhhh](https://user-images.githubusercontent.com/84547558/152064104-73183bfb-fe48-4eb7-ab34-0078af000e24.png)

