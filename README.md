# API-Challenge
This challenge uses python to examine global weather through analysis with scipy and numpy libraries, and visualization with pandas, matplotlib, and gmaps.

![Global Temperature](https://github.com/bakerv/API-Challenge/blob/main/Images/GlobalMax%20Temperature%20(F)vslat.png)

## Data 
Live forecast data was pulled from the OpenWeatherMap API for a random sampling of cities around the globe. The GooglePlaces API was used to find hotel data for cities with ideal weather conditions.

![OpenWeatherMap API Call](https://github.com/bakerv/API-Challenge/blob/main/Images/API_codesample.PNG)

### Work Cited:
CityPy was used to generate city names from a set of random coordinate pairs. Thank you Winston Chen.

## Analysis
### Correlation Table, Northern Hemisphere
![Correlation Table](https://github.com/bakerv/API-Challenge/blob/main/Images/NH_Correlations.PNG)

There is a strong correlation between the maximum forecasted temperature and degrees latitude of a given city. This relationship was stronger for the northern hemisphere than the Southern Hemisphere. This correlation makes senses, cities nearer to the equator experience more solar exposure and more consistent heating through out the year. As latitude increases, cities experience increasingly more dynamic changes in solar exposure and heating through out the year. These higher latitude areas receive less solar energy overall.

![Max Forecasted Temperatures](https://github.com/bakerv/API-Challenge/blob/main/Images/NH_Max%20Temperature%20(F)vslat.png)


There is a moderate negative correlation between maximum forecasted temperature and humidity. This makes sense when you consider inland plains and desert regions. These areas are dry with low humidity, but have high daytime temperatures. This relationship breaks down in coastal areas or near other large bodies of water. These areas become extremelly humid with high temperatures due to increases in evaporation off of these large bodies of water. 

![Humidity Comparisons with Gmaps](https://github.com/bakerv/API-Challenge/blob/main/Images/HumidityMap.png)

There is a weak positive correlation between cloudiness and humidity. The weak nature of this relationship makes sense when you consider thunderstorms in inland dry regions, and continual humidity in coastal regions. Dry regions will experience a positive change in humidity when a storm passes through, and then a negative change in humidity when the skies are clear. In contrast, coastal regions can experience extreme humidty without a cloud in the sky

The next step in this analysis would be to test this hypothesis. This could be done by conducting on another round of analysis on data divided between coastal and inland cities. I expect we would see different correlations for each of these groups.
