On this project, we will answer this question: What is the weather like as we approach the equator?

# Part 1: WeatherPy
Create a Python script to visualize the weather of over 500 cities of varying distances from the equator. 

## Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
Use OpenWeatherMap API to retrieve weather data and create a series of scatter plots to showcase the following relationships:

- Latitude vs. Max Temperature

- Latitude vs. Humidity

- Latitude vs. Cloudiness

- Latitude vs. Wind Speed

## Requirement 2: Compute Linear Regression for Each Relationship
Compute the linear regression for each relationship. Separate the plots into Northern Hemisphere and Southern Hemisphere. 

### create the following plots:

- Northern Hemisphere: Temperature vs. Latitude

- Southern Hemisphere: Temperature vs. Latitude

- Northern Hemisphere: Humidity vs. Latitude

- Southern Hemisphere: Humidity vs. Latitude

- Northern Hemisphere: Cloudiness vs. Latitude

- Southern Hemisphere: Cloudiness vs. Latitude

- Northern Hemisphere: Wind Speed vs. Latitude

- Southern Hemisphere: Wind Speed vs. Latitude

Explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover

# Part 2: VacationPy
Use the cities csv file created in Part 1 and plan a vacation.

- Create a map that displays a point for every city in the city dataframe. The size of the point will be humidity in each city
- Narrow down the dataframe to find your ideal weather condition
- Create a new DataFrame called hotels_df to store the city, country, coordinates, and humidity
- For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates
- Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image

## References
- ChatGPT: Convert the Unix timestamp in 'Date' column to datetime and format it as 'yyyy-mm-dd'
city_data_df['Date'] = pd.to_datetime(city_data_df['Date'], unit='s').dt.strftime('%Y-%m-%d') and
timestamp = city_data[0]['Date']
Graph_date=datetime.utcfromtimestamp(timestamp).strftime('%Y-%m-%d')
- ChatGPT: Fixed issue with the spacing: params["filter"] = f"circle:{lon},{lat},{radius}"
