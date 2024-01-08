# Lancaster County Housing Market Analysis

Analysis of the Lancaster County NE housing market focusing on the geographical role contributing to a house's price.

## Description

The project was completed as a group as part of a class assignment. The data has all house sales in Lancaster County between 2016-2023 and includes information such as square footage, quality, CDU, number of bedrooms, etc. The data was retrieved by the Lancaster County Assessor Office.
The data preprocessing was completed in Python and the regression and analysis were completed in R.

## Anaylsis

### Data Preprocessing

The [first step](Latitude_Longitude_Extraction.ipynb) was to geocode the address of each of the sales. OpenMapStreet API was used to retrieve the longitude and latitude of each of the addresses. The data was also cleaned removing null values and outliers.  

The [second step](K-Means-Clustering.ipynb) was to create neighborhoods or clusters to sort the address into. K Means Clustering was used to achieve this.

The [third step](Closest-Features-Extraction.ipynb) was to create a list of points of interest in Lancaster County and return the distance from those points of interest to each of the addresses.

### Regression and Analysis

The regression and analysis were done in R by another team member. We used linear regression and ridge regression. We were able to create a model that could predict house prices with an r-squared of .7847. Some of the variables used include distance to points of interest such as airport or downtown, cluster, year built, total living area, bedrooms, etc. 
Some of the results can be found in the regression and analysis folder.
## Authors

Angeline Luther  
Mark Pham  
Elizabeth Weber
