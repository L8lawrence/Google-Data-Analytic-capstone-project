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

# Process
Cleaning and preparing data for analysis.

. Created a column called "ride_length."
. Created a column called "day_of_week."
. Calculated the day of the week that each ride started using the "WEEKDAY" command (for example, =WEEKDAY(C2,1)) in each file. Format as General or as a number with no decimals, noting that 1 = Sunday and 7 = Saturday.

Some of the collected data set were too large to process with excel so i used R programming language for further and easier processing of the data set.
