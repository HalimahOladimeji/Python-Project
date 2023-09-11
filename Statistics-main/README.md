# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This is a project about exploring different APIs and using the information gotten to build models.
We aim to analyze bike sharing data, explore local points of interest and build a model to understand their relationships.


## Process
Step 1: Connecting to CityBikes API
I first explored the CityBikes API.
I worked on the city London in Great Britain and extracted the bike station data whilst using lists and dictionaries.
I parsed the data using python and libraries like requests and pandas and stored it in a Pandas DataFrame. 
Then I transformed and analyzed the data using the Dataframe.
Step 2: Connecting to Foursquare and Yelp APIs
I extended my analysis by connecting to Foursquare and Yelp APIs.
I queried these APIs for POI information in the vicinity of bike stations.
I organized and stored the retrieved data in separate DataFrames.


## Results
I compared the data coverage from both APIs and found out Yelp worked better for my location especially since my POIs were business based like restaurants.
 I also evaluated the number of bike stations covered and ensure that the relevant 	stations are included.
I assessed the quality of the CityBikes API data by evaluating factors such as data accuracy and completeness. I compared this result with the Yelp APIs to identify any discrepancies or differences.
I created a new dataframe with the combination of both data and I visualized the data. This helped in visualizing the proximity of POIs to the stations.
I created a regression model using python which demonstrates a relationship between the number of bikes in London and the number of slots available.
OLS Regression Results                            
==============================================================================
Dep. Variable:                  Bikes   R-squared:                       0.262
Model:                            OLS   Adj. R-squared:                  0.261
Method:                 Least Squares   F-statistic:                     282.6
Date:                Mon, 11 Sep 2023   Prob (F-statistic):           1.72e-54
Time:                        03:58:04   Log-Likelihood:                -2716.9
No. Observations:                 797   AIC:                             5438.
Df Residuals:                     795   BIC:                             5447.
Df Model:                           1                                         
Covariance Type:            nonrobust                                         
====================================================================================
                       coef    std err          t      P>|t|      [0.025      0.975]
------------------------------------------------------------------------------------
const               18.4955      0.485     38.121      0.000      17.543      19.448
Total bike slots    -0.4880      0.029    -16.811      0.000      -0.545      -0.431
==============================================================================
Omnibus:                       94.717   Durbin-Watson:                   1.756
Prob(Omnibus):                  0.000   Jarque-Bera (JB):              129.784
Skew:                           0.891   Prob(JB):                     6.57e-29
Kurtosis:                       3.857   Cond. No.                         31.3
==============================================================================

## Challenges 
Connecting to the different APIs 
Finding the best visualization to use during analysis


## Future Goals
I would try to explore more POIs and see if more relationship can be found
I would also study other cities and other related data in the APIs

