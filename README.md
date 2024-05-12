# python-api-challenge

## WeatherPy and VacationPy Analysis

This Jupyter Notebook code provides an analysis in two parts: WeatherPy and VacationPy.

### What do you need?

- Python 3.x
- Jupyter Notebook
- Pandas
- Matplotlib
- Citipy
- GeoViews
- Geoapify API
- OpenWeatherMap API

### Part 1: WeatherPy

This jupyter notebook contains the code to visualize the weather of over 500 cities of varying distances from the equator. The analysis utilizes the 'citipy' Python library and the OpenWeatherMap API.

The code uses the OpenWeatherMap API to retrieve weather data from the cities list and creates a series of scatter plots to showcase relationships between latitude and weather variables such as temperature, humidity, cloudiness, and wind speed.

Linear regression is computed for each relationship. The plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). The code also includes linear regression lines, the model's formula, and the r values in the plots.

### Part 2: VacationPy

This jupyter notebook contains the code to use weather data to plan future vacations. It utilizes the Geoapify API to create map visualizations.

The code creates a map displaying a point for every city in the city_data_df DataFrame, with the size of the point representing the humidity in each city.

The code narrows down the city_data_df DataFrame to find cities with ideal weather conditions, such as max temperature lower than 27 degrees but higher than 21, wind speed less than 4.5 m/s, and zero cloudiness.

For each city, the code uses the Geoapify API to find the first hotel located within 10,000 meters of the city's coordinates. It then creates a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.

### How to use the code?

1. Clone the repository to your local machine.
2. Open the Jupyter Notebook file - WeatherPy.ipynb and VacationPy.ipynb - using Jupyter Notebook.
3. Run each cell sequentially to execute the analysis and view the results.
