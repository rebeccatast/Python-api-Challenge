# Weather Visualizations and Vacation Planning

**Part I - WeatherPy**

I used this Python script to build visualizations of the weather for over 500 cities from around the world. Using Python libraries and an OpenWeatherMap API, this script can show weather patterns such as Max Temperature, Humidity, Cloudiness, and Windspeed for cities at various points of latitude from around the globe. This script primarily uses scatter plots and multiple regression analysis to show relationships for the following:
  - Temperature vs. Latitude
  - Humidity vs. Latitude
  - Coudiness vs. Latitude
  - Wind Speed vs. Latitude
  - Relationship between Temperature vs. Latitude for the Northern Hemisphere
  - Relationship between Temperature vs. Latitude for the Southern Hemisphere
  - Relationship between Humidity vs. Latitude for the Northern Hemisphere
  - Relationship between Humidity vs. Latitude for the Southern Hemisphere
  - Relationship between Cloudiness vs. Latitude for the Northern Hemisphere
  - Relationship between Cloudiness vs. Latitude for the Southern Hemisphere
  - Relationship between Wind Speed vs. Latitude for the Northern Hemisphere
  - Relationship between Wind Speed vs. Latitude for the Southern Hemisphere
  
The script also provides a CSV output of all retrieved data and a PNG image for each scatter plot. 

**Part II - VacationPy**

Using the data collected in Part I, I planned an ideal vacation spot based on weather patterns. Using jupyter-gmaps and Google Places API, I created a heat map displaying the humidity for all cities collected in Part I. In addition, the script helped me to narrow down potential vacation spots with the following criteria:

  - Max temperature less than or equal 85 but greater than or equal to 75 degrees
  - Wind speed less than 10 mph
  - Cloudiness index that is less than 30%
  - Humidity level that is less than 65%
  
After narrowing down the top vacation spots based on the above conditions, the script uses Google Places API to find the first hotel for each ideal vacation city located within 5000 meters of your citys' coordinates. The returned hotel coordinates are then plotted on the humidity heatmap.
