# Final Report

## 1. Introduction
-----
#### Established in 2016, Cyclistic is a bike-share offering service located in Chicago, USA. Cyclistic currently offers more than 5,800 bicycles that are geo-tracked and locked into a network of over 690 stations across Chicago. The bikes can be unlocked from one station and returned to another station in the system anytime.

#### As of August 2021, Cyclistic offers the following pricing plans (USD):

- Single ride passes \\$3.30 per trip
- Full day passes, \\$15 per day
- Annual memberships, \\$9 per month

#### The Cyclistic team have recently concluded that annual memberships are more profitable than casual riders. Furthermore, the team have noted that while 30\% of users use the bikes for their work commute, the majority of Cyclistic users ride for leisure. This report will assess how existing Cyclistic causal riders can be encouraged to convert to annual memberships.



## 2. Process
----
#### Cyclistic have provided historical trip data to be analysed. For the purpose of this analysis, only data between August 2021 and July 2022 will be assessed. The license to use this dataset can be located [here](https://ride.divvybikes.com/data-license-agreement).

#### There are around 100,000 - 500,000 entries for each month saved under their own CSV. Due to the large file sizes, Python has been used to clean and process the large datasets. There is minimal human error and data bias since the primary, structured, historical data is taken from the bikes themselves. However, due to data privacy rules, there is no data relating to the type of user.

#### The data has been cleaned by way of merging all 12 datasets into one, deleting incomplete data elements, removing outliers, removing negative ride lengths and summarising the dataset by date and time variables. The full data cleaning process has been documented in “Data Cleaning Process”.

#### The data cleaning process highlighted that there are missing values regarding the station id and station name which take up over 15% of the data. Since removing 15% of the rows will affect the analysis, the column of station id and station name is removed in the data cleaning process.

#### The cleaned dataset has been saved under the file name "all_trips_cleaned".

## 3. Analysis
----
### 3.1 Most popular stations


![popularity_of_station1.png](attachment:popularity_of_station1.png)

#### The map demonstrates that the shoreline bike stations centered around the Navy Pier are the most popular. Navy Pier is known as a famous tourist place in Chicago where people spend time there for leisure. This confirms Cyclistic’s internal analysis that the majority of its users ride for leisure.

#### Interacting with the map highlights that the southern stations are Cyclistic’s least popular stations despite the stations covering a large surface area. This indicates that only a small proportion of Cyclistic users use the bikes to commute to and from more residential areas, and instead the vast majority of users use the bikes around the central, tourist locations of Chicago.

### 3.2 Most popular time of year

![total_ride_by_weekday_and_month.png](attachment:total_ride_by_weekday_and_month.png)

#### The above calendar heatmap shows that the summer months are the most popular time of the year for Cyclistic, and weekends are the most popular time of the week. Summer is the time where people usually go on vacation and weekend is the time people spend their leisure time. This indicates that the majority of users are riding for leisure purposes.

### Casual Riders

![casual_ride_by_weekday.png](attachment:casual_ride_by_weekday.png)

### Member Riders

![member_ride_by_weekday.png](attachment:member_ride_by_weekday.png)

#### Separating the heatmap by casual and member riders shows that members use the Cyclistic service more consistently throughout the year and week, whereas casual riders tend to only use the bike service during the summer months on the weekend.

#### The most popular date for casual rider is 14th August 2021, which is a Saturday. While the most popular date for member rider is 14 July 2022, Thursday. The pattern of casual riders ride more on weekend and member riders ride more on weekday may indicate that members are using the Cyclistic service for their work commute and other daily activities unlike casual riders whom are using the Cyclistic service for predominately leisure purposes. 

#### Moreover, the first three popular date for casual riders are in 2021, while member riders first four popular dates are distributed equally between 2021 and 2022. It could be argued that casual riders feeling more comfortable visiting tourist destinations after a long period of covid stay home order, which lead to more rides in 2021 summar compared to 2022 summar. 

### 3.3 Most popular time of day

![trips_count_by_hours.png](attachment:trips_count_by_hours.png)

#### The stacked bar plot shows that 6pm is the most popular time of day for Cyclistic users, with the most common time of day being 17:08:31 for casual riders and 17:18:23 for members. The significant increase of member riders using the bikes at 8 a.m. and later on around 6 p.m. suggests that a lot of member riders are using the Cyclistic service for their work commutes.

#### Although member riders ride more than casual rider, the ride length of casual rider are longer than the ride length of member rider's ride length. This further strengthens the argument that casual riders use Cyclistic bikes for leisure purposes.



## 4. Recommendations

#### As identified in the client brief, the marketing recommendations concluded from the insights of this case study should not be focused on encouraging new customers to use the Cyclistic bike service but instead focus on encouraging casual riders to convert to annual memberships.

#### The three possible marketing recommendations for Cyclistic are as follows:

#### 1. Digital campaign which shows Cyclistic bike’s being used in a Chicago local’s everyday life

#### Section 3.3 identified that the most common time of day for casual and member riders was 6 p.m., and the most popular time of day for casual riders is similar to member riders which is during the day with a slight peak during work commute times. This insight highlights that there are casual riders using the Cyclistic service for their work commute without investing in an annual membership. To encourage casual riders to become members, a digital campaign which encourages Chicago locals to observe how Cyclistic fits into their every day life would be beneficial. This would also help change public opinion that Cyclistic is a predominantly tourist service. In addition, it will help spread consumer demand across the city rather than focusing bike usage around the Navy Pier of Chicago.

#### 2. Notifications/email reminders for casual riders to observe the price benefit of annual memberships

#### Similar to the insight noted in recommendation 1, for Chicago locals to choose to invest in an annual membership rather than regularly purchasing casual trips with Cyclistic, phone notifications and email reminders should be used to remind regular casual riders (most likely Chicago locals) of the long term pricing benefit from investing in an annual membership rather than purchasing regular casual trips.

#### 3. Digital campaign showing the benefits of using a Cyclistic bike in a post-COVID-19 society

#### Section 3.2 concluded that there has been an increase in casual rider using the bike service post COVID-19. This insight could be highlighted by Cyclistic in which riding bikes outdoors can improve people's health as well as lower the chances of getting infected by COVID-19 or other kind of virus. 
