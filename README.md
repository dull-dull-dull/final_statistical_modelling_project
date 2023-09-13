# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Searching for points of interest (breweries) based on their proximity to public bikes around Toronto


## Process
Pulled location of all public bikes in Toronto via CityBikes API.

Pulled location of all breweries within 1km of a bike station via Foursquare API.

Pulled location of all breweries within 1km of a bike station via Yelp API.

EDA

Merged and cleaned business listings

EDA for modelling

Modelling



## Organization
'notebooks/city_bikes.ipynb' contains CityBikes API call, EDA, data cleaning, and dataframe building.

'notebooks/yelp_foursquare_eda.ipynb' contains FourSquare and Yelp API calls, EDA, data cleaning, and dataframe building.

'notebooks/joining_data.ipynb' contains dataframe joining, further EDA and data cleaning, and SQLite database work.

'notebooks/model_building.ipynb' contains paiplot correlation analyses and linear regression models.

'notebooks/data/' includes:
'df_bikes.csv', containing bike stations in Toronto.
'fsq_results.csv', containg all results returned in the FourSquare API call
'fsq_results_unique.csv', containing cleaned FourSquare data with each duplicate listed only in relation to its nearest bike station.
'yelp_results.csv', containg all results returned in the Yelp API call
'yelp_results_unique.csv', containing cleaned Yelp data with each duplicate listed only in relation to its nearest bike station.


## Results
FourSquare API provides extensive listings – roughly equivalent to Yelp – but with marginally less business information.


In assessing the relationships between geographic location and rating, as well as geographic location and distance from a bike station, no meaningful trends emerged.


This may be due, in part, to the limited variables made available for analysis – methods for addressing this are addressed in 'Future Goals', below.



## Challenges 
Limited variables, particularly numeric variables, limited the options for model building.


## Future Goals
Yelp's API contains other methods for pulling detailed business information.


In this iteration of the project, I pulled business listings from both FourSquare and Yelp to generate a more complete list of results.


With more time and resources, particularly greater access to Yelp API calls, I would query FourSquare for business listings and Yelp for details about those listings. This should provide a more robust dataset with greater opportunities for analysis.