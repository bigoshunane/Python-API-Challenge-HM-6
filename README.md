# World Weather Analysis

The aim of this project is to develop Python Script which can visualize:
1. The weather of 500+ cities across the world of varying distance from the equator.
2. Plan future vacations based on this weather data anaysis.
 
To accomplish this, a [simple Python library](https://pypi.org/project/citipy/) and 
the [OpenWeatherMap API](https://openweathermap.org/api) are used to create a representative model of weather across cities in the world.

Python script developed ,cities data and figures are in the repository under file names Images, WeatherPy and VacationPy and output_data.

To run the code:

   -  Install citypy in your python environment (https://pypi.python.org/pypi/citipy)
   -  Save OpenWeatherMap API Key (https://openweathermap.org/) as 'weather_api_key'
   -  Google API Key (https://console.developers.google.com/getting-started) as 'g_key'
   -  Create API Keys and store it in the 'api_keys.py' file before running the Jupyter notebooks.

## Part.I  WeatherPy

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

## Part.II VacationPy

Report includes:

1. Create a heat map that displays the humidity for every city generated from Part.I WeatherPy.

2. Narrow down the DataFrame to find your ideal weather condition, by intruducing the following parameters:

   -  A max temperature lower than 90 degrees but higher than 70.
   -  Wind speed less than 10 mph.
   -  Zero cloudiness.
    
## Final observable trends summary

-  Figure reports:

    -  Temperature (F) vs Latitude.

![tvl](https://user-images.githubusercontent.com/84547558/152062547-5444d87e-e639-4129-aa0c-23c050f539f6.png)

-  Fig.1 The scatter plot shows highest maximum temperature were recorded at lower latitude values, 
           as latitude increases temperature drops this is due to the fact   that the lower the latitude 
           the closer we get towards the equator; hence, the higher the temperature and viceversa. 
    
   -  Humidity (%) vs Latitude.
 
![hvl](https://user-images.githubusercontent.com/84547558/152062807-af960fe0-6074-42ce-bf31-26347c1b5074.png)
 
-  Fig.2 The scatter plots shows low humididty at polar regions and as latitude gets higher 
           humidity increases in the souther hemisphere.

    -  Cloudiness (%) vs Latitude.

![cvl](https://user-images.githubusercontent.com/84547558/152062943-621ebb4a-144c-4829-aea1-64e44c01a2aa.png)

-  Fig.3 The scatter plot shows evenly distributed data points across the latitude ; hence, 
           there is no difference in cloudiness as the cities as farther or closest  to the equator.

    -  Wind Speed (mph) vs Latitude.

![wvl](https://user-images.githubusercontent.com/84547558/152063035-8b00ee76-400b-4861-b7cb-73efc11b1871.png)

-  Fig.4 The scatter plot of wind speed and latitude shows no observable pattern 
            that can describe the relationship between them. 

      -  Northern Hemisphere - Temperature (F) vs Latitude.
 
 ![tvln](https://user-images.githubusercontent.com/84547558/152063154-86fff225-c514-417c-96d9-e305ef486d3c.png)
 
 -  Fig.5  The linear regression model between temperature and latitude for north hemisphere cities
            show strong negative correlation where temperature is higher at lower latitude and starts 
            dropping as we go away from the equator i.e. as latitude gets higher.

       -  Southern Hemisphere - Temperature (F) vs Latitude.
 
 ![tvlsh](https://user-images.githubusercontent.com/84547558/152063246-331018cc-d22c-40d5-a8d8-9d9607e82514.png)
 
-  Fig.6  In southern hemisphere the regression shows that there is moderate positive correlation between
           temperature and latitude but not as observed in nothern hemisphere.

     -  Northern Hemisphere - Humidity (%) vs Latitude.
 
![hlpn](https://user-images.githubusercontent.com/84547558/152063410-1d10f73e-83b1-4e17-8119-2c0f3ba48e5f.png)

-  Fig.7  The regression depicts that there exists moderate correlation between humidity
            and latitude in northern hemisphere.

     -  Southern Hemisphere - Humidity (%) vs Latitude.
 
 ![hlshh](https://user-images.githubusercontent.com/84547558/152063527-a76b8fc7-a9ab-47fd-b6f3-2e51e0f0297d.png)
 
-  Fig.8  The regression of humidity vs latitude in southern hemishphere shows weak negative correlation.

     -  Northern Hemisphere - Cloudiness (%) vs Latitude.
 
 ![ctn](https://user-images.githubusercontent.com/84547558/152444637-aa8dfc58-ff0a-4e17-bb5b-abaf0d6023dc.png)
 
-  Fig.9  The regression shows that there is higher cloudiness in norther hemisphere at higher latitudes.
 
     -  Southern Hemisphere - Cloudiness (%) vs Latitude.
 
![shcc](https://user-images.githubusercontent.com/84547558/152063865-80dc4aaa-d21c-40d5-adbf-600ebdfd810d.png)

-  Fig.10  The regression between cloudiness and latitude in southern hemisphere shows that there exists 
             not much correlation between the data points.

     -  Northern Hemisphere - Wind Speed (mph) vs Latitude.
 
 ![wns](https://user-images.githubusercontent.com/84547558/152064022-49ed22e4-aebd-42e1-9e91-13f19aec9ec7.png)
 
-  Fig.11  The regression plot of wind speed and latitude shows that there 
             is weak positive relationship between wind speed and latitude.
 
     -  Southern Hemisphere - Wind Speed (mph) vs Latitude.
 
![hhhh](https://user-images.githubusercontent.com/84547558/152064104-73183bfb-fe48-4eb7-ab34-0078af000e24.png)

-  Fig.12  The regression plot of wind speed and latitude in souther hemisphere shows 
            negative weak correlation between wind speed and latitude.

    -  Heat map that displays the humidity for every city generated.

![hmmm](https://user-images.githubusercontent.com/84547558/152066485-412653b8-0649-4f6f-bd0f-44cb87885d9d.png)

-  Hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

![mhm](https://user-images.githubusercontent.com/84547558/152066649-836a7649-37df-4cdf-83bc-ffc05595b810.png)



##  Final observable trends summary:

Generally the lower the latitude the closer it gets towards the equator therfore the higher the temperature: as a result, maximum temperatures for cities appeared to have direct inverse relationship with latitude, but not equally across northern and southern hemispheres. Southern Hemisphere climates tend to be slightly milder than those at similar latitudes in the Northern Hemisphere. This is because the Southern Hemisphere has significantly more ocean and less land and water heats up and cools down more slowly than land. 

The southern hemisphere tends to have higher humidity in general while northern hemisphere tends to have decreasing maximum temperatures as we go further away from the equator. There were not strong correlations between latitudes and humidity, cloudiness, and wind speed based on the latitude of the cities, which makes a good sense.

From vacationPy analysis we can create exploratory-interactive geospatial, weather information, heat maps and visualization through Google API, and other similar API applications to play a remarkable role in exploiting the potential socio-economic values from available large datasets.

In addition to vacation place other potential decisions can be also made applying different enquiries to the given dataset.



## References
Raw data was provided by © 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.

© 2021 Trilogy Education Services, LLC, a 2U, Inc. brand. Confidential and Proprietary. All Rights Reserved.
