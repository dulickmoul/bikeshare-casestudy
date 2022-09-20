
# Bike share case study
## Case Study: How Does a Bike-Share Navigate Speedy Success?

### Google Data Analystics Professional Certification Program - Capstone Project

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

![union](https://user-images.githubusercontent.com/113184507/191272748-9788fa32-fdd4-4a8e-bb98-8ccb41c3869d.png)
- Inspecting the data
![1](https://user-images.githubusercontent.com/113184507/191273193-9fadbd77-043e-4f99-b82b-2b04c6d5605c.png)
- Cleaning and organizing
![organized](https://user-images.githubusercontent.com/113184507/191273403-ae42ab3d-73b5-42de-a53f-f649d80662fe.png)
![cleantoosmallduration](https://user-images.githubusercontent.com/113184507/191273566-dafebbdf-5387-4b11-8998-d9f055c7f622.png)
![checking1](https://user-images.githubusercontent.com/113184507/191273679-53fb828a-424a-4112-8b5f-924a94dba928.png)
Analyze Phase
- Descriptive Analysis
- Comparison between members and casual riders
![summary](https://user-images.githubusercontent.com/113184507/191274911-40a8b1ad-9384-4b87-9c1e-877b99e6f132.png)

- Average duration per user type sorted by day of the week
![rides_byweekday](https://user-images.githubusercontent.com/113184507/191273906-d09678d3-a4ba-4a83-b03f-05bf63fede3f.png)
- Average duration per user type sorted by time of the day
![rides_bydatetime](https://user-images.githubusercontent.com/113184507/191274309-1e6add32-a2fa-4140-96d0-ae675eab6c27.png)
- Number of rides through out the year group by month
![rides_bymonth](https://user-images.githubusercontent.com/113184507/191274484-61c065a8-71cc-4748-aa6c-c5f9603ac12b.png)
- Number of rides by bike types
![bike_types](https://user-images.githubusercontent.com/113184507/191274646-3b1fc00c-dfe2-41aa-ad77-facb2857c2e1.png)
- Top 20 popular routes
![top20routes](https://user-images.githubusercontent.com/113184507/191274748-5e2618f9-f110-4d48-8121-3e4fa68fa8a5.png)

Share Phase
- Visualizations by Tableau

![number_rides_by_user_type](https://user-images.githubusercontent.com/113184507/191275149-ea8f8a2b-e29a-46ec-9f88-3c77e09d7b80.png)

![average_rides_length_by_minute](https://user-images.githubusercontent.com/113184507/191275165-5376eb9e-ba79-46e9-85ea-02c4750c6697.png)

Total number of rides grouped by user type. As you can see currently the number of casual users is lower than that of member riders. But the average ride duration time per minute is higher (25.64 minutes) than the member type (12.27 minutes)

![different_ride_time (1)](https://user-images.githubusercontent.com/113184507/191275363-3d06e86a-aa99-4929-b79e-fe8c5500ba5f.png)

The graph showing the number of rides by hours of the day grouped by user type. As we can be, both group of users have the most rides from 15:00pm to 19:00pm, and then by the time frame from 6:00-9:00am the second largest number rides. The 0:00-5:00 time frame has the fewest rides

![WEEKDAY_RIDES](https://user-images.githubusercontent.com/113184507/191275692-a168ae0e-7de0-497b-ad22-4be83d96d0c3.png)

The chart shows the number of riders of 2 user types by different days of the week. We see a slight difference, for the casual type group there are more riders on weekends on Saturday and Sunday and lower weekdays. Particularly for members type, weekdays have the most riders, Sunday is the day with the fewest riders

![Total _rides_by_month](https://user-images.githubusercontent.com/113184507/191275836-909293de-c89a-484e-b489-5db38efd1103.png)

The chart shows number riders of 2 user types group by month. The difference between the 2 groups is not much. July-September has the most riders. The number of riders gradually decreased from October to April of the following year. To understand the reasons behind this behavior, we also need to learn more about the geography, the weather where the analysis was performed, Chicago. After learning that July-September is summer in Chicago, the weather began to warm up, suitable for cycling. In contrast, for the months from November-March is the winter time when the outdoor temperature is gradually colder, so it affects cycling. As the outdoor climate warms up from April, there is a resurgence in riders. The good weather is positively correlated with the number of riders.

![bike_type](https://user-images.githubusercontent.com/113184507/191275968-dce8ab04-5a1c-43a5-ade5-11674ab80c8c.png)

The chart shows the behavior in choosing the type of bikes of 2 groups of users. Both groups had the largest selection of classic bikes, second largest choice is electric bike Particularly for docked bikes, only casual groups choose but not by member rider. This different behavior needs to investigate deeper to find the reason behind it.
![top20routes](https://user-images.githubusercontent.com/113184507/191276161-f85fe83a-4ce7-42b8-8d1c-dc6aad794b60.png)

Top 20 routes with the most rides, grouped by user type. As we can see, Streeter Dr & Grand Ave and DuSable Lake Shore Dr & Monroe St have the most casual riders. This may determine a number of strategies to attract casual riders to become member riders later on.

Act Phase

Now that we have finished creating visualizations, it’s time to act on our findings and proposing the top 3 recommendations based on our analysis:
- Marketing: Summer is the busiest season of the year for Cyclistic, as the weather gets warmer. Organizing events or competitions, this is the best time for advertising activities and campaigns. They can be conducted nearby equestrian hotspots. Classic bikes are used the most, therefore services can be created for those people.

- Weekend membership : As we noticed that most casual riders are on weekends. More activites or better deals are necessary to attract casual riders to become members.

- Discounts: Cyclistic can host cycling competitions with exciting prizes and can offer annual membership discounts to participants.

Conclusion: 
The differences in the behavior of casual and member types are not so much. The data clearly shows that casual riders often cycle on weekends and that cycling times are also higher than member riders. Member riders can show their passion and the consistent for cycling activities throughout the week.

### Contact info: [Linkedin](https://www.linkedin.com/in/du-lick-moul)  
















