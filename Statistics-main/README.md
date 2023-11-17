# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This is a project about exploring different APIs and using the information gotten to build models.
We aim to analyze bike sharing data, explore local points of interest and build a model to understand their relationships.

Process
Part 1: Connecting to CityBikes API

Tasks:

1.) I had chose New York City as my city of choice and had retrieved all available bike stations in that city 2.) I had used the API to call the latitude, longitude and number of bikes for each bike station. Then I had parsed my JSON response into a Pandas dataframe which I had also converted to CSV

Part 2: Connecting to Foursquare and Yelp APIs
Tasks:

1.) I had connected to the Foursquare API + Yelp API. 2.) For each of the bike stations in Part 1, I had queried both APIs to retrieve information for Restaurants 3.) Next I had created a DataFrame for the Yelp results and Foursquare results. 4.) I prefered Yelp API as it allows customization and was easy to use

Part 3: Joining Data
Tasks:

1.) I had joined the data from Part 1 with the data from Part 2 to create a new dataframe and had also converted to csv 2.) I had then started cleaning data + EDA visualizations 3.) I had created my own SQLite database and stored the data I had collected 4.) I had also validated my data.

Part 4: Building a Model
Tasks:

1.) I had build a regression model that resembles a relationship with the number of bikes and POI(restaurants) characteristics
## Process
Step 1: Connecting to CityBikes API
I first explored the CityBikes API.
I had chosen Hamilton Ontario as my city of choice and had retrieved all available bike stations in that city 
I had used the API to call the latitude, longitude and number of bikes for each bike station. 
Then I had parsed my JSON response into a Pandas dataframe which I had also converted to CSV

Step 2: Connecting to Foursquare and Yelp APIs
I extended my analysis by connecting to Foursquare and Yelp APIs.
I queried these APIs for POI information in the vicinity of bike stations.
I organized and stored the retrieved data in separate DataFrames.
I preferred Yelp because it provided more information

Step 3: Joining Data
I had joined the data from Part 1 with the data from Part 2 to create a new dataframe and had also converted to csv
I had then started cleaning data andEDA visualizations 
I had created my own SQLite database and stored the data I had collected 
I had also validated my data.

Step 4: Model building
A regression model was built using Python's statsmodels to analyze the relationship between bike availability and POI characteristics. In summary, my regression analysis did not yield satisfactory results for predicting the number of total bikes based on the variables I considered. It appears that my current model may not be the best fit for this prediction task. Further investigation and potential model refinement may be required to improve my predictive capabilities.

## Results
I compared the data coverage from both APIs and found out Yelp worked better for my location especially since my POIs were business based like restaurants.
I also evaluated the number of bike stations covered and ensure that the relevant 	stations are included.
I assessed the quality of the CityBikes API data by evaluating factors such as data accuracy and completeness. I compared this result with the Yelp APIs to identify any discrepancies or differences.
I created a new dataframe with the combination of both data and I visualized the data. This helped in visualizing the proximity of POIs to the stations.
I created a regression model using python which demonstrates a relationship between the number of bikes in Hamilton and the number of slots available.

## Challenges 
Connecting to the different APIs 
Finding the best visualization to use during analysis

## Future Goals
I would try to explore more POIs and see if more relationship can be found
I would also study other cities and other related data in the APIs

