# python-api-challenge
Part One: WeatherPy Script
This Python script visualizes the weather of over 500 randomly generated cities from varying distances from the equator. After citipy was used to generate said list, a series of scatterplots were generated to illustrate the relationship between latitutde and various other measures, including: max temperature (in Farenheit), humidity, cloudiness, and wind speed. The results are show below: 

![image](https://user-images.githubusercontent.com/119253324/219884626-516f61b8-2199-4f04-8033-af55ddcc2a7d.png)
![image](https://user-images.githubusercontent.com/119253324/219884635-812d2be4-2878-4861-bb86-7a962a69ac9c.png)
![image](https://user-images.githubusercontent.com/119253324/219884641-0f00a061-8c7e-499f-b94b-3fa9998c9449.png)
![image](https://user-images.githubusercontent.com/119253324/219884649-fee43744-4745-490c-9f35-2937fe97054f.png)



Next, the cities were separated into those located within the Northern and Southern hemispheres. A series of linear regression plots were then created to illustrate the correlation between latitutde and max temperature (in Farenheit), humidity, cloudiness, and wind speed. The results are show below: 

![image](https://user-images.githubusercontent.com/119253324/219884685-2edbb398-eaad-4418-b344-f5f8cb3a5d8a.png)
![image](https://user-images.githubusercontent.com/119253324/219884696-31cc4443-a1a7-4077-8c32-661787fcde55.png)

**Discussion about the linear relationship:** The above scatterplots were generated with the intent of measuring the correlation between latitude and max temperature (in fahrenheit), first for cities located within the Northern Hemisphere, and subsequently for cities located within the Southern Hemisphere. 

This evaluation revealed a relatively strong negative correlation between max temperature and latitude for cities located in the Northern Hemisphere. The calculated correlation coefficient r, which quantifies the degree of the linear relationship between the two variables being measured, was roughly -0.85. This indicates a relatively strong trend between lower (colder) temperatures as the cities' geographic location moved farther North.

The calculated value of r between the variables of latitutde and max temperature for cities located in the Southern Hemisphere was approximately 0.48. This communicates a weak positive correlation between the variables, revealing a loose, general trend of rising max temperatures as the city location moves from the South Pole towards the equator. 


![image](https://user-images.githubusercontent.com/119253324/219884719-a20bdbf1-bf0b-4ebb-a871-4ea24f0428fc.png)
![image](https://user-images.githubusercontent.com/119253324/219884725-f9d2212e-5369-4066-ae97-476220f91943.png)

**Discussion about the linear relationship:** The above scatterplots were generated with the intent of measuring the correlation between latitude and humidity, for cities located in the Northern and Southern Hemispheres. The calculated r values were roughly 0.35 and 0.36, respectively. This indicates a very weak positive correlation between the measures. Given this figure, no trend is readily apparent. 


![image](https://user-images.githubusercontent.com/119253324/219884745-99a91bc6-443a-4b1b-8197-f2787ddfd5ca.png)
![image](https://user-images.githubusercontent.com/119253324/219884751-72494b2d-8b3f-4826-b050-7cb7ab44a4f1.png)

**Discussion about the linear relationship:** The above scatterplots were generated with the intent of measuring the correlation between latitude and cloudiness, for cities located in the Northern and Southern Hemispheres. The calculated r values were roughly 0.37 and 0.44, respectively. This indicates a very weak positive correlation between the measures. Given this figure, no trend is readily apparent. 

![image](https://user-images.githubusercontent.com/119253324/219884765-f012c45e-e20c-4cf8-a034-e05c2b98b1c1.png)
![image](https://user-images.githubusercontent.com/119253324/219884782-cb605a20-3290-4614-9303-536fcef7d0e1.png)

**Discussion about the linear relationship:** The above scatterplots were generated with the intent of measuring the correlation between latitude and wind speed, for cities located in the Northern and Southern Hemispheres. The calculated r values were roughly 0.13 and -0.33, respectively. This indicates a very weak positive and negative correlation between the measures. Given this low degree of correlation, no trends are readily apparent. 


**Part Two: VacationPy Script
This script uses the weather data generated in the WeatherPy script to create map visualizations using the geoViews Python library and the Geoapify API.

First, a map was created to display a point for every city, with the relative size of the point refelcting the city's humidity. The result is below: 
<img width="857" alt="image" src="https://user-images.githubusercontent.com/119253324/219884945-9e388df0-2d77-40b7-a690-a1b4889466f4.png">

Next, the dataframe of cities was edited to filter out cities with an average temperature outside of the range of 50-78 degrees farenheit. GeoApify was used to identify the closest hotel to each latitutde and longitude, and a map was created to plot this data geographically. 
<img width="631" alt="image" src="https://user-images.githubusercontent.com/119253324/219885072-35ed816d-49ac-4601-aedb-22405c67f0c5.png">

Next, the dataframe of cities was edited to filter out cities with an average temperature outside of the range of 50-78 degrees farenheit. GeoApify was used to identify the closest hotel to each latitutde and longitude, and a map was created to plot this data geographically. 
