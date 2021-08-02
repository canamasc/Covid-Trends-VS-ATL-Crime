# Covid-Trends-VS-ATL-Crime
Georgia Tech Data Science Bootcamp Project 1

Purpose: Explore correlation between new COVID case trends and crime rate trends accross 5 NYC boroughs in the time period of Feb 2020 through Sep 2020. 
ORIGINAL IDEA WAS TO DO THIS FOR ATL NEIGHBORHOODS BUT WE COULD NOT FIND COVID DATA AT A LOWER LEVEL THAN BY COUNTY FOR THE STATE OF GEORGIA.

Data cleaning (NYC_Data_Cleaning.ipynb) uses files:
- NYC / COVID-19_Daily_Counts_of_Cases__Hospitalizations__and_Deaths.csv
- NYC Crime Dataset1 CSV.csv
- NYC Crime Dataset2 CSV.csv
- NYC Crime Dataset3 CSV.csv
- NYC Crime Dataset4 CSV.csv
- NYC Crime Dataset5 CSV.csv

Concatenates all crime data sets, gets rid of unneeded columns, trims date ranges in both sources to match, standardizes date format and merges the two sources on DATE. 

Pandas / Matplotlib / Google API work (NYC_Crime_COVID.ipynb):

- Uses groupby, aggregate functions, merges, sorts to look at how crime trends, crime type distributions, covid trends, and crime/covid correlations vary by different factors like sex, race, and time period. 
- Charts findings using matplotlib (scatter chart + linear regression model, pie charts, line charts)
- Uses Google Maps API calls to plot crime heat map for 5 NYC boroughs
