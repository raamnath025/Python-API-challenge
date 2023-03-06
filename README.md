# Part 1: WeatherPy
In this deliverable, I created a Python script to visualize the weather of over 500 cities of varying distances from the equator. I used the citipy Python library, the OpenWeatherMap API, and my problem-solving skills to create a representative model of weather across cities.

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination was utilized.

## Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
To fulfill the first requirement, I used the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, I created a series of scatter plots to showcase the following relationships:
- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

## Requirement 2: Compute Linear Regression for Each Relationship
To fulfill the second requirement, the linear regression was computed for each relationship. The plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). I found it helpful to define a function in order to create the linear regression plots.

Next, a series of scatter plots were created. I made sure to include the linear regression line, the model's formula, and the r values.

I created the following plots:
- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

After each pair of plots, I explained what the linear regression was modeling. I also described any relationships that I noticed and any other findings I uncovered.

# Part 2: VacationPy
In this deliverable, I used my weather data skills to plan future vacations. Also, I used Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and the CSV file loaded with the weather and coordinates data for each city created in Part 1 was used to get started.

## My main tasks was to use the Geoapify API and the geoViews Python library and employ my Python skills to create map visualizations.

- I first created a map that displayed a point for every city in the city_data_df DataFrame. The size of the point is the humidity in each city.
- Then, I narrowed down the city_data_df DataFrame to find my ideal weather condition using the following:
    - A max temperature lower than 27 degrees but higher than 21
    - Wind speed less than 4.5 m/s
    - Zero cloudiness
- I created a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

- For each city, I used the Geoapify API to find the first hotel located within 10,000 meters of my coordinates.

- FInally, I added the hotel name and the country as additional information in the hover message for each city on the map
