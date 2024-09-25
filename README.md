# Airplane Risks Analysis Project


## Project Overview

This project deals with a company that wants to venture into another business so as to expand their portfolio.The company is intrested in aviation, specifically an entreprise that purchases planes and use them for commercial and private purposes. They however do not know the risks that are associated with this type of business and that hinders their decision making. My project is aimed at looking into the risks associated with operating this type of business.


## 1.1 Business Understanding

The Business at hand deals with airplanes which touches on broad fields. Since the business targets both public and private business plans, the stakeholders in the business will be of a wide range. The Company itself is a stakeholder, the companies selling the airlines, the airports they will be operating in, the passengers, the crew who will handle the business and the government in the country of operation are all stakeholders.

### 1.2 Project Goal

My project aims at Knowing the types of airplanes used in commercial and private entreprises and their aggregate against Total uninjured
passengers.I am using the number of uninjured passengers to gauge the lowest risk.

*who are the Air service providers with the highest uninjured passengers?

*What plane models are not prone to accidents?

*what models that have good safety features? 

*How many engines and what type of engines are good for our business?.

At the end I will give actionable insights that will help the board to make a decision.

## 2.1 Data Understanding
For my project, I am working with data that has already been collected by other data scientists. The data is stored in **kaggle** where it is updated oftenly and is made accessible to everyone who wants to do research with it. The data is stored in a **csv format** inside a folder named 'data'. When we read the data to our notebook using the pandas library, we get a dataframe as our output. The dataframe has 90348 rows and 31 columns. The columns define our data by giving the differnt fields their names while the rows hold the information of different columns.From a quick look at the dataframe, we know that the data we are dealing with is from investigation of aircraft accidents. We have both continous and categorical data, with the latter making the most part of our data. Out of 31 columns, 26 columns are made up of categorical data. The categorical data is in object form while the contious data is in float form.

## 3.1 Data Cleaning
My dataset in the original form is not ready for me to use in my analysis. The data has missing values, unnecessary columns and duplicates in it. After doing my data understanding, I went into cleaning my data. I started by making a copy of our original data for future reference if I will need to look at original data. I Checeked for duplicate and dropped them, leaving only one unique row in cases where the rows were duplicated. I studied my columns and dropped that will not be relevant for my project.I checked for null values and discovered that our data had missing values in 30 columns. For continous data, I filled the missing values with a **mean** because it **reduces bias and maintains relationship between our data**. For my categorical data, I filled the missing values with an placeholder, name **Unknown**. Droping the rows with missing values would have led to me losing 90% of my data and it would affect the quality of my research.

## 4.1 Explorative Data Analysis
After cleaning my data, it is now ready for analysis and visualization When doing analysis, often you compare hwo different variables affect an outcome. To investigate the various relationships between variables in our data, we use the **.groupby() method** which helps us to group the columns together and do aggregation. Since the project is specific to aircrafts for business, I went to the aircraft column and specified that I only want to deal with airplanes alone in my analysis. I perfomed various groupby functions using **'Total.Uninjured** as my aggregation element. Since we want to pinpoint the aircrafts with the lowest risk, I  used uninjured people as my metric for measuring the level of risk in this project. After grouping data in various categories, I came up with visualizations to help in interpreting the grouped data. This is the link to my Visualizations;
https://public.tableau.com/app/profile/victor.masinde/viz/ProjectDashboard_17272562308670/PrjoectDashboard?publish=yes


## 5.1 Conclusion

I grouped my data by **Model** and checked how the model of the plane affects safety of passengers incase of an accident. Different models in After plotting a bar graph, we find that model MD 83 has the highest number of uninjered passengers.**model MD 83** is the Model with the least risks.

I went further and grouped my data by **Air.carrier** to check and see how adifferent Air carriers can affect the rate at which passengers remain uninjured incase of an incident or accident.Differenent companies have diferent ways of operating their planes and this can dertermine the level of injuries incase of accidents. After visualization below,we find that the Singapore Airlines, Ltd' has the highest number of uninjered passengers.**Singapore Airlines** is the Air carrier with the least risks.

I took my Airplane data and grouped by **number of engines** .In this step,we look at the effect that the number of engines in an aircracft has on safety of passengers. Here there is no linear relationship. When doing our reccomendations we will leave out this column as it does not help us make an informed decison. The scatter plot below shows that there is no relationship between the two variables.

We go further and ivestigate how grouping planes by the **purpose of flight** affects the rate of passengers being injured in an incident or incindent.Different business types calls for different designs of planes and therefore it is important to look into this category. The business that we want to venture in, is intrested in Executive/corporate and Public Aircraft. These two fall under the category of aircrafts with low risks in that they perfom well in the number of players uninjured. Aircrafts involved in other activitiess such as skydiving and gliding has low number of injuries.

I did another Groupby by **Engine Type**. Differnt Planes run on different engine types and they can sometimes affect the occurence and magnitude of accidents. From our Bar graph visualization, we see that passengers are more likely to be safe in planes with a **Turbo fan** as compared to other planes as it has the highest number of passengers who were uninjured.

Grouping by **Injury Severity** enables us to ascertain under what type of accidents are we likely to have high injuries or low injuries. This enables the comapny to make necessary precautions on it. Injury severity has been grouped into different levels depending on the magnitude of the accident. We take this and compare it with our total uninjured passengers. From the visualization, the highest number of passengers that were not injured fall under **fatal(11)**. Theis shows that more people were saved from fatal accidents than all the other catergories and incidents. Such a finding shows that the response quick and awareness from the crew to the accident was high.

## 6.1 Recommendations
After completing data analysis, the recommendations from the study are as follows:

* Based on our findings, I strongly recommend that the head of the new aviation division focuses on buying the MD 83 model aircraft to be used in their new business.

* I recommend that the head of the new aviation division buys aircracft that runs on Turbo fans type of engines.

* I strongly reccomend that the head of the new aviation division Focus on using the aircrafts they will purchase only for commercial and private businesses to reduce their exposure to risk. 

* I strongly recommend that the head of the new aviation division puts emphasis in training their crew on matters of safety and evacuation in order to know how to deal with different challenges and prevent or reduce loss by minimizing risk.