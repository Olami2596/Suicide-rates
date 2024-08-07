# Suicide Rate Analysis Report

This is a report on the suicide rates of countries involved in a survey from 1985 to 2016 provided in the dataset named which was gotten from the World Health Organization (WHO) in the form of a csv file. The dataset used for the analysis was provided and downloaded locally.

## Features of the dataset

The dataset contained 27840 rows and 9 columns which are listed below:

- Country 

- year 

- sex 

- age 

- suicides_no  

- population 

- gdp_for_year ($) 

- Unnamed: 7 

- 8 Unnamed: 8 

## Data Wrangling

Before I started wrangling the data, I made a copy of the data and viewed it.


I then proceeded into dropping the Unnamed 7 and 8 columns because they were irrelevant to the analysis after which I dropped the null values in the dataset


While trying to convert the gdp_for_year ($) column from object to int I discovered certain strings that did not contain numbers so rows containing such strings had to be dropped

A function was then created to remove the comma’s in the gdp_for_year ($) column before it could be converted to int 

I then converted the suicides_no column from object into int

The age column was in object format so that had to be changed and since it was also given in a range I got the mean value for each range and added that column into the dataset and dropped the age column.

## Conclusions
- The top 5 countries are Russian Federation, United States, Japan, Ukraine, France and the bottom 5 countries are Oman, Macau, Maldives, Antigua and Barbuda, San Marino

- Correlations between suicides, GDP per capita and population.

A pairplot was first created to visualize the correlation between them then a correlation matrix was also created to see the numerical correlation.

There wass no strong correlation between suicides, GDP per capita and population.

- Using appropriate visual notation to visualize total suicides over years. 

The suicide rates increased during the years 1985 - 1994.

The suicide rates fluctuated between the years 1995 - 2011 and there was a sharp decline in the suicide rate after the year 2011.

- Comparison of suicides by gender over years

The suicide rates for the male gender are far higher than that of the female gender as shown in the line plot above though the male and female gender experienced a rapid increase and decrease at the same point in time along the years 

- Calculate and Visualize suicides on generation and on age group.

Generation Z had the highest suicide rates among all the ages while Generation A had the lowest suicide rates amongst all the generations.

 Mean ages of 9.5 had the lowest suicide rates and the highest suicide rates was found in the mean ages of 44.5

