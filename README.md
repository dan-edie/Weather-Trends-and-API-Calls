# python-api-challenge
Project that examines weather trends as locations approach the equator.

This project uses Python code and API calls to pull weather information and city locations using both 
OpenweatherAPI and citipy.

Random latitude and longitude coordinates are generated and passed to CityPy. If a city is located at these
coordinates, it is stored; if no city is located then the code skips those coordinates.

The city list is then passed to the OpenweatherAPI, and weather data is stored in a Pandas dataframe.

From there, we filter for specific weather criteria. First, outlier data where humidity is over 100% is
removed as necessary. Then, several plots are created to look for any correlation between weather patterns
and latitude and longitude in both the North and South hemispheres.

Linear correlations were plotted in the final portion of the project to look for any trends. The results
are discussed in the project.
