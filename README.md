# **Behavioral Analysis for Rental Bike users**

 **Summary:** Cyclistic is a fictional bike company. They have two types of customers: casual riders and annual members. Casual riders are those who only purchased single ride passes and full day passes. Then, riders who purchased annual membership are labelled as annual members. The marketing director believes in order to maximize profits, we need to convert casual riders to annual members. The objective of this project is to discover the different behaviors between casual riders and annual members.

 **Tools:** Python, Jupyter Notebook, Pandas and Matplotlib

View my Python code here in [Github](https://github.com/carolinenata/divvy_bikes/blob/main/divvy.ipynb)

## Steps

For this project, I am going to use Python (Jupyter Notebook) and its packages (Pandas and Matplotlib) for exploratory analysis and visualization. I will use the six steps data analytics process that we learned in the course, which are:

1. Ask

2. Prepare

3. Process

4. Analyze

5. Share

6, Act

## Ask

These are the three questions prior our analysis: 

*How do annual members and casual users use Cyclistic bikes differently?

*Why would casual members buy Cyclistic annual membership?

*How can Cyclistic use digital media to influence casual users to become members? 

## Prepare

For this analysis, I am going to analyze 12 Cyclistic customer data (the most recent 12 months). My data spans from June 2022 - May 2023. Click this link to visit to the source where I downloaded the data from. 

## Process

For the process, I will be using Visual Studio Code to run Python. I imported all 12 CSV files using Panda on the Jupyter Notebook.  After that, I concat them all into one file for analysis. 

Note: Unfortunately, not all columns in this data are necessary for analysis. I have to remove some columns like start_lat, start_ing, end_lat, end_lng because I don't see how they are relevant to my analysis. I also removed the duration column because some of the data shows '####' value instead of time value. I'm going to manually add a new 'duration' column in Python later. Lastly, I remove rows with N/A or null values. 

## Analyze

View my Python code here in [Github](https://github.com/carolinenata/divvy_bikes/blob/main/divvy.ipynb)

Here are the notable discoveries I found during my analysis: 

* Saturday is the most popular for annual members while Wednesday is the most popular day for casual riders. While most annual members rent more on weekdays, casual riders rent more on weekends. 

* Classic bike is the most popular bike among both types of members. More annual members use electric bike than casual riders. However, docked bike is only used among casual riders and never been used by annual members. 

* The most popular starting and ending station for both member and casual riders is Streeter Dr & Grand Avenue. 

* There are more annual members than casual riders in the 12 CSV files. 

* Casual riders rent  longer more than annual members. The maximum duration for annual members is one day while the maximum duration for casual riders is 22 days.

## Share

**Amount of Casual Riders vs Annual Members**

<img width="568" alt="casual annual" src="https://github.com/carolinenata/portfolio/assets/138493962/dffaeb7f-38d9-4296-9ae2-35ca7c2117da">

There are 1,7 million Casual Riders and 2,7 million Annual members in this dataset. To maximize our profits, we have to convert Casual Riders to Annual members.

**Rideable Type for Casual Riders and Annual Members**

<img width="571" alt="bikes" src="https://github.com/carolinenata/portfolio/assets/138493962/585cf4f9-676c-4ae5-94fe-a855875679c7">
Even though classic and electric bikes are popular among both users, it turns out that only casual riders use docked bike. This is very eye opening because there is a chance we can utilize the docked bike to convert existing casual users to members. However, we also need to realize that existing members don't use the docked bike at all. 

**Most popular day for Casual Riders and Annual Members**

<img width="501" alt="most popular day" src="https://github.com/carolinenata/portfolio/assets/138493962/354a6cba-13c4-48a6-882d-72dbb372fdb7">

From this graph, we can see that Wednesday is the most popular day for members while Saturday is the most popular day for casual riders. We know that most members rent the bike during weekdays, while most casual riders rent the bikes more on weekends. 

**Boxplot Duration for Casual Riders and Annual Members (Excluding the Outlier)**

<img width="440" alt="duration 2" src="https://github.com/carolinenata/portfolio/assets/138493962/40c66f30-6bb1-4c1b-a876-323eff7bba8c">

This boxplot only includes the MIN, FIRST QUARTILE, MEDIAN AND THIRD QUARTILE. We learn that casual riders have higher median, first and third quartile than members. We can conclude that casual riders  use the bike more longer than the members. 

**Boxplor Duration for Casual Riders and Annual Members (Including the Outlier)**

<img width="507" alt="duration" src="https://github.com/carolinenata/portfolio/assets/138493962/154eb088-b22a-4d99-8aaa-fbcd91a99a19">

This boxplot includes the MAX duration of members and casual. As you can see, the max duration for casual is much higher in casual than members. (1498 minutes aka 1 day and 58 minutes for members & 32,035 minutes aka 22 days,5 hours and 55 minutes for casual). 

## Act

### How do annual members and casual members behave differently?

Annual members rent the bike during weekdays while casual riders rent the bike during weekends. On average, casual riders rent the bike longer than annual members. Also, casual riders uses the docked bike while annual members don't use it at all. We know that most members rent their bike to commute. In this case, we can conclude that casual riders rent their bikes more for leisure than work. 

### Why would casual members buy Cyclistic membership?  

Here are some ways we can convert casual riders into members: 

* Cyclistic can set up a bicycle community gathering event on the weekend to invite more casual riders to participate. During the event, they could make a special promotion for their annual membership. For example, casual riders who sign up to be a member on the event can get a special discount (they pay less than the original price for the annual membership because of the event discount). 

* Cyclistic may offer a 'free-trial' kind of offer for casual members. For example, we can give active casual riders an annual membership privilege for one week. These casual riders can rent our bike for weekdays and weekend with annual membership price. If the casual riders feel the convenience of using the bike for work, eventually they will sign up for annual membership so they can take the bike everyday to work. 

* Since most casual riders use the bike in the weekend, Cyclistic can offer them special price single or full day passes on certain holidays (Christmas, New Year etc) if they sign up to be annual members.

### How can Cyclistic use digital media to influence casual users to become members? 

There are a few things we can do:

* They can make a social media campaign targeted towards corporate commuters. They can upload their stuff during weekdays after work so the targeted group can see their content. Not only casual riders, but they can make this campaign as an opportunity to attract people who are willing to use a bike to go to work. For example, they can promote the benefits of riding a bike to work like reduce traffic, eco-friendly, reduce risk of cardiovascular diseases and etc.

* We can do referrals in socials. New casual riders who is interested to get annual membership can get a discounted price if they follow Cyclistic's socials (e.g, Instagram page) and tag their 3 friends to convince them to try using Cyclistic or convert into a member. The friend that has been tagged AND successfully converted annual membership will get a discount as well for signing up.

* Make a small competition in social media for the annual members. Encourage annual members to make content about the positive benefits becoming a Cyclistic member through Reels and Tiktok. Cyclistic can pick the top 5 winners (most beloved or viral content) and give them a discount for annual membership renewal. 
