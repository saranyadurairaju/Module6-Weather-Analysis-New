# Weather and Vacation Analysis with API

An API (stands for Application Programming Interface) is a software that allows two or more applications to connect with each other.  In simple words, it is the messenger that delivers your request to the provider and then delivers the response back to you. It is an interface that allows one application to talk to another one through simple commands.

* Ease of  integration
* Better integration
* Automating tasks
* Improved services
* Innovation

## Overview of Project

Jack works for PlanMyTrip Application company and they are interested to find the weather of the cities around the world as the travelers are interested to choose cities accordingly. Also, they will help them find a better vacation itinerary. So finding the right hotel with preferred weather and helping them with the route map is important. So, in this module we are going to use API's especially weather and google APIs to find all the necessary details. So, we are finding the below details:

  *	Weather data retrieval. 
  *	Customer Travel Destinations Map creation.
  *	Travel Itinerary Map creation.
   
## Analysis 

Before we start doing our Analysis, we need to setup the dependencies Panda and Numpy libraries in our code to work with Data and Calculations. We have to load the file with the path and use .read function of Panda to read the data. Below are the extra dependencies we need specifically for APIs.

![image](https://user-images.githubusercontent.com/85472349/126910203-70e1e1c4-2f75-4529-b313-3d0c14bf2e4b.png)
  
### Weather Database

In this we are generating a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data which we gathered, we have to use API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

![image](https://user-images.githubusercontent.com/85472349/126912437-c5c49b23-8f0b-46f4-8389-8de518bb3d7d.png)

![image](https://user-images.githubusercontent.com/85472349/126912479-8a1d5efd-7007-4d4b-b29a-5dadf4ae8062.png)

![image](https://user-images.githubusercontent.com/85472349/126912483-c59ad402-081c-466d-8e13-cdc07a9ad453.png)

### Vacation Search

We are using the database we created with the list of cities to find the location and other details. First, we have to use the input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

![image](https://user-images.githubusercontent.com/85472349/126912724-ec58d177-2d10-4b53-b030-3423804c155f.png)

![image](https://user-images.githubusercontent.com/85472349/126912741-21edd286-2aa1-40dd-9c97-a587be933936.png)

### Vacation Itinerary

To find the Vacation Itinerary, we are using the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

![image](https://user-images.githubusercontent.com/85472349/126912867-c607f8c8-82cc-4703-8bb6-9623d5ff5de1.png)

## Results

Here are the links for each delivery and the corresponding datas or maps: 

#### Weather Database

The database which we create using all the **weather API** info looks like below dataframe:

![image](https://user-images.githubusercontent.com/85472349/126912999-2d08f6cc-1c43-499f-800a-1c6da4dea8b2.png)

The Weather_Database folder with Weather_Database.ipynb and WeatherPy_Database.csv files can be found in the below link:

https://github.com/saranyadurairaju/Module6-Final-Assignment-Analysis/tree/main/Weather_Database

#### Vacation Search

The database which we created with the weather info including the **Hotel name** looks like below:

![image](https://user-images.githubusercontent.com/85472349/126913020-ad36ba1a-1d7f-4006-bee0-5ec67cc15ebd.png)

The Vacation_Search folder with the Vacation_Search.ipynb file, WeatherPy_vacation.csv file and WeatherPy_vacation_map.png image is :

https://github.com/saranyadurairaju/Module6-Final-Assignment-Analysis/tree/main/Vacation_Search


#### Vacation Itinerary

The dataframe with the **Four Cities** information for the vacation itinerary: 

![image](https://user-images.githubusercontent.com/85472349/126913039-7842dabe-ed59-4b12-9ec8-0892c9f5c662.png)

The Vacation_Itinerary folder with the Vacation_Itinerary.ipynb file, WeatherPy_travel_map.png and WeatherPy_travel_map_markers.png image is the following:

https://github.com/saranyadurairaju/Module6-Final-Assignment-Analysis/tree/main/Vacation_Itinerary


__I hope Jack and his team has found all the information they want to give for the travelers. And the PlayMyTrip App is user friendly for everyone to find weather and vacation details.__
