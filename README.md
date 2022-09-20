## Bike share case study
Case Study: How Does a Bike-Share Navigate Speedy Success?

Google Data Analystics Professional Certification Program - Capstone Project

Table of contents 
- Introduction
- Ask Phase
- Prepare Phase
- Process Phase
- Analyze Phase
- Share Phase
- Act Phase
- Conclucions

Introduction: 

Scenario:
You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations. 

Company: Cyclistic a bike-share company in Chicago.
Business objective: maximizing the number of annual memberships
Data Analysts task: how casual riders and annual members use Cyclistic bikes differently 
  Casual riders: riders who purchase single-ride or full-day passes 
  Member riders:  annual members (riders who purchase an annual unlimited membership)
Consider key stakeholders:
● Cyclistic: A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day.

● Lily Moreno: The director of marketing and your manager. Moreno is responsible for the development of campaigns and initiatives to promote the bike-share program. These may include email, social media, and other channels.

● Cyclistic marketing analytics team: A team of data analysts who are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy. You joined this team six months ago and have been busy learning about Cyclistic’s mission and business goals — as well as how you, as a junior data analyst, can help Cyclistic achieve them.

● Cyclistic executive team: The notoriously detail-oriented executive team will decide whether to approve the recommended marketing program

Ask Phase
Three questions will guide the future marketing program:
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

Prepare Phase
Data Description: download 12 months data of cyclistic trip from October 2021 to September 2022. The dataset consists of twelve separate ‘.csv’ formatted files representing each month. The datasets are located in the  Link: Index of bucket "divvy-tripdata"

ride_id,
started_at, 
 ended_at, 
 rideable_type,
 start_station_name, 
 start_station_id, 
 end_station_name, 
 end_station_id,
 start_lat, 
 start_lng, 
 end_lat,
 end_lng, 
 member_casual
 
Tools: BigQuery SQL and Excel for data cleaning and analysis

Process Phase
- Union the data
