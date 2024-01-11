# Google-Data-Analytic-capstone-project
# Introduction

Welcome to the Cyclistic bike-share analysis case study! This capstone project is the final project in my Google Data Analytics Professional Certificate course. In this case study I will be analyzing a public dataset for a fictional company provided by the course. I will be using R programming language for this analysis because of its easy statistical analysis with easy code chunks and data visualizations.

# Case Study Overview
#  Scenario
You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.
About the company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.
# ASK

.Goal

Design Marketing strategies aimed at converting casual riders into annual members.

. Business Task

Identify how annual members and casual riders use Cyclistic bikes differently.

. Key Stakeholders

Lily Moreno: The director of marketing and your manager.

Cyclistic marketing analytics team: a team of data analysts responsible for collecting, analyzing, and reporting data.

Cyclistic executive team.

. Data Sources

The data has been made available by Motivate International Inc. under this license.
# Prepare
The dataset follows the ROCCC  below:

Reliable - yes, not biased

Original - yes, can locate the original public data

Comprehensive - yes, not missing important information

Current - yes, dataset is updated monthly

Cited - yes

. Key tasks

1. Download data and store it appropriately.
 
Data was downloaded and copies stored securely on my computer 

2. Identify how it’s organized.
 
The data is in CSV (comma-separated values) format, and there are a total of 13 columns.

3. Sort and filter the data.
 
 For this analysis, I used data for the last 10 months (Jan 2023 - Oct 2023) because it is more current from when i did my analysis.

4. Determine the credibility of the data.

For the purpose of this case study, the datasets are appropriate and will enable me to answer the business questions. 

Deliverable

A description of all data sources used
Source of data - Cylistic Bike Share company.

    Load individual dataset


#3. Process
Data processing and Cleaning is done using R programming 

. Created a column called "ride_length."
. Created a column called "day_of_week."
. Calculated the day of the week that each ride started using the "WEEKDAY" command (for example, =WEEKDAY(C2,1)) in each file. Format as General or as a number with no decimals, noting that 1 = Sunday and 7 = Saturday.

Some of the collected dataset were too large to process with excel so i imported the data into R programming language for further processing, data manipulation and analyzing of the data set. 

. Removed rows with ride length that is <0. The data frame includes a few hundred entries when bikes where taken out of docks and checked for quality by Divvy where ride_length was negative or "zero". As identified in section 3.2 there were a few invalid data points with ride lengths less than 0. These data points should be deleted from the cleaned dataset. 
. Remove incomplete and blank rows. 
### 4.2 Remove incomplete and blank rows
There were a few instances where there were no recorded station names. These incomplete rows of data should be removed.
#I notice that the data frame contains rows with incomplete informations like started_at , ended_at , 
#started_at_id and ended_at_id have incomplete rows that should be removed 
### 4.4 Remove duplicates 
The ride_id column is unique to each ride. This column is reviewed for any possible dublicate to be removed.
### 4.5 check for and remove missing NA values.
They where no missing NA values in the data set.

#Analyze
Data Aggregation is carried out within the R script and here are the following steps taken to achieve descriptive results.
1. Perform descriptive analysis on riders ride lentgh covered
2. Perform descriptive analysis on riders distance by knowing thier ride distance covered
3. Converted the started_at and ended_at to date time object to get the ride_length in secs

  ## Key Insights...
. Member riders  use the bikes more often than casual riders based on the ride counts.

   ![Rplot](https://github.com/L8lawrence/Google-Data-Analytic-capstone-project/assets/149658921/6d09d77a-f165-4122-9c6a-6f0434e93e42)

    
   

. From the visuals below you can see that casual riders spend more time on the bikes than member riders whom spend consistent time on weekdays but more on wknds. 
. Member riders use bikes more on thursday and fridays.

   ![Rplot01](https://github.com/L8lawrence/Google-Data-Analytic-capstone-project/assets/149658921/9d02cd72-f14c-45fd-8e17-76d7536c15dd)

. Exported the cleaned data into a Tableau tool for visualisation for further analysis and insight 

## Share
. From the visuals below, you can see that member riders have more rides than casual riders.

. Both member and casual riders started experiencing a significant increase in the usage of the rides from Feb - April 2023 
![T](https://github.com/L8lawrence/Google-Data-Analytic-capstone-project/assets/149658921/f89bdf8a-4b10-4765-aeda-65f09861d373)


. Casual riders spend more time on the bikes on weekends compare to member riders but spend lesser time riding during weekdays.

. Member riders spend more time on bikes on week days.


![Captureee](https://github.com/L8lawrence/Google-Data-Analytic-capstone-project/assets/149658921/ff9d8cf1-e5f9-4a26-a36e-db6fbb4bbdf4)

#### Distance Traveleved by casual and member riders
. From the visiallz below you can see that casual riders covered  a longer distance while riding compared to member riders that covered a shorter distance with a difference in few killometers. 

![AV distance](https://github.com/L8lawrence/Google-Data-Analytic-capstone-project/assets/149658921/30d07b8a-b78b-490b-a289-3637e546ab61)

### Rideable bike type vs rider type comparison 
. Both member and casual users use the classic bike more often .how ever only casual member use the ducked type .
