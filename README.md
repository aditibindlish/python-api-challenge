# APIs OpenWeather and GeoMaps
**This project consists two parts, analysing Weather and using that to decide possible Vacation locations.

***Part 1: Weather Analytics
In this part, have created a Python script to visualize the weather of over 500 cities of varying distances from the equator. Hsve used the citipy Python library and APIs to create a representative model of weather across cities.


****Analysis: Plots Showcasing relationship between Weather Variables and Latitude, using the OpenWeatherMap API to retrieve weather data from the cities list generated. Created a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

***Part 2: Computed Linear Regression for Each Relationship
Computed the linear regression for each relationship, separated the plots into Northern Hemisphere and Southern Hemisphere and defined defined a function to reduce repetition.

Following plots were created alongwith an analysis based on the plots:

Northern Hemisphere: Temperature vs. Latitude

Southern Hemisphere: Temperature vs. Latitude

Northern Hemisphere: Humidity vs. Latitude

Southern Hemisphere: Humidity vs. Latitude

Northern Hemisphere: Cloudiness vs. Latitude

Southern Hemisphere: Cloudiness vs. Latitude

Northern Hemisphere: Wind Speed vs. Latitude

Southern Hemisphere: Wind Speed vs. Latitude


***Part 2: Vacation ANalytics
In this part, have used weather data generated to plan future vacations. Also, used  geoViews Python library, and the Geoapify API to create visualisations.


--Created a map that displays a point for every city in the city_data_df DataFrame with the size of the point depicting the humidity in each city.
--Narrowed down the city_data_df DataFrame to find ideal weather condition with temp in the ramnge of 19-26 degreees celcius and humidity less than 28%.

--Created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

--For each city, used the Geoapify API to find the first hotel located within 10,000 meters of city coordinates.

--Added the hotel name and the country as additional information in the hover message for each city on the map.

