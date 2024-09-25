# Airplane Risks Analysis Project


## Project Overview

This project deals with a company that wants to venture into another business so as to expand their portfolio.The company is intrested in aviation, specifically an entreprise that purchases planes and use them for commercial and private purposes. They however do not know the risks that are associated with this type of business and that hinders their decision making. My project is aimed at looking into the risks associated with operating this type of business.


## Business Understanding

The Business at hand deals with airplanes which touches on broad fields. Since the business targets both public and private business plans, the stakeholders in the business will be of a wide range. The Company itself is a stakeholder, the companies selling the airlines, the airports they will be operating in, the passengers, the crew who will handle the business and the government in the country of operation are all stakeholders.

### Project Goal

My project aims at Knowing the types of airplanes used in commercial and private entreprises.What plane models are prone to accidents.I also aim to know if the accidents due to human error or plane condition. The frequency of accidents and losses in this business is important therefore I want to know how often are plane accidents. At the end I will give actionable insights that will help the board to make a decision.

## Data Understanding
For my project, I am working with data that has already been collected by other data scientists. The data is stored in **kaggle** where it is updated oftenly and is made accessible to everyone who wants to do research with it. The data is stored in a **csv format** inside a folder named 'data'. When we read the data to our notebook using the pandas library, we get a dataframe as our output. The dataframe has 90348 rows and 31 columns. The columns define our data by giving the differnt fields their names while the rows hold the information of different columns.From a quick look at the dataframe, we know that the data we are dealing with is from investigation of aircraft accidents. We have both continous and categorical data, with the latter making the most part of our data. Out of 31 columns, 26 columns are made up of categorical data. The categorical data is in object form while the contious data is in float form.

## Data Cleaning
My dataset in the original form is not ready for me to use in my analysis. The data has missing values, unnecessary columns and duplicates in it. After doing my data understanding, I went into cleaning my data. I started by making a copy of our original data for future reference if I will need to look at original data. I Checeked for duplicate and dropped them, leaving only one unique row in cases where the rows were duplicated. I studied my columns and dropped that will not be relevant for my project.I checked for null values and discovered that our data had missing values in 30 columns. For continous data, I filled the missing values with a **mean** because it **reduces bias and maintains relationship between our data**. For my categorical data, I filled the missing values with an placeholder, name **Unknown**. Droping the rows with missing values would have led to me losing 90% of my data and it would affect the quality of my research.

## Explorative Data Analysis
After cleaning my data, it is now ready for analysis and visualization When doing analysis, often you compare hwo different variables affect an outcome. To investigate the various relationships between variables in our data, we use the **.groupby() method** which helps us to group the columns together and do aggregation. Since the project is specific to aircrafts for business, I went to the aircraft column and specified that I only want to deal with airplanes alone in my analysis. I perfomed various groupby functions using **'Total.Uninjured** as my aggregation element. Since we want to pinpoint the aircrafts with the lowest risk, I  used uninjured people as my metric for measuring the level of risk in this project. After grouping data in various categories, I came up with visualizations to help in interpreting the grouped data. This is the link to my Visualizations.

