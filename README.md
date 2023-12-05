# python-api-challenge
API challenge

The API challenge has two parts - WeatherPy and VacationPy. 
In WeatherPy, 
- we are generating a list of 500+ random cities using the citipy library. 
- By using the list of cities generated, we are sending requests to the open weather API for each city in the list and get the response to parse the data. Populate all the required information like latitude, longitude, max temp, humidity, cloudiness, wind speed, country, and date to a list for each of the cities which we will use to create a dataframe.
- Using the data from the dataframe, we create scatter plots for Latitude vs - 
        i) Maximum temperature
        ii) Humidity
        iii) Cloudiness
        iv) Windspeed.
- We divide the cities data into northern and southern hemisphere and compute the linear regression of both the hemispheres to plot the charts for Latitude vs the parameters mentioned above. We calculate the correlation coefficient for each of them to determine the strength in their relationships and to find any difference in the pattern in the both the hemispheres.

In VacationPy,
- We use the hvplot in pandas to plot the cities data collected in WeatherPy on a map.
- We are planning a vacation and idetifying the cities that we would want to go to based on the temperature, cloudiness and windspeed. 
- After identifying a set of cities which have our required weather conditions we are finding a hotel nearest to our destination in each of the cities using the geoapify API. 
- We are plotting the hotels on the map using hvplot to display the hotel name, city, and country. Now we have narrowed our list to specific locations along with accomodation details.