# Taxi Trips
## A dashboard of the public Chicago Taxi Trip dataset

Link to dashboard: https://datastudio.google.com/reporting/c0c36b16-356e-4198-b8d2-8a6123657faa <br />
Link to dataset:  https://www.kaggle.com/datasets/chicago/chicago-taxi-trips-bq <br />

### Dataset Overview

This dataset is collected in Chicago, Illinois, which is in the United States with data from 2013 to the present day. <br />
This dataset tracks the taxi cabs in Chicago, which are operated by private companies and licensed by the city. <br />
Most of the taxicab trips are reported to a regulatory agency in Chicago, which then collects these information. <br />
Some of the data features include the taxi id, trip length, distance, fares, tips, etc.


## Analysis
![image](https://user-images.githubusercontent.com/99934518/209703049-7d763ac8-c2a7-47cd-9547-c13e34f2f860.png)

To start off, this is a simple analysis of the data and here is a very general overview. <br />
In general, when taking a taxi trip, we would like to know of some of these details displayed here. <br />
First, for each reported trip, the average fare is $15.62, and the average tips earned for these drivers is $1.42. <br />
The average trip length is roughly 3.2 miles (or ~5km) and the average trip time is about 12.4 minutes. <br />
Some data cleaning is performed to make the data more representative and accurate. <br />
Trips that are at $0 and above a certain threshold (In this instance, $100) and trips below 50 miles are filtered out. <br />
These simple statistics may even be quite useful in telling us some things. <br />
Some conclusions drawn is that the average trip is quite short, of about 3.2 miles (or 5km) only. It also takes 12.4 minutes
for the trip, and you could perhaps even estimate traffic and congestion from these statistics. <br />
For this distance covered, the average fare is $15.62, which can be quite pricey for this short trip, and the customers generally tip quite generously,
roughly 9% of their fares. <br />
To extrapolate, they can even be used to get insights on the customers' affluency, willingness to pay for these rides, culture, or even draw comparisons
to other states or countries. <br />
<br />

Next, we may likely be curious of the companies that make up majority of these taxicab trips. <br />
the null values are removed from the company list,  which may belong to smaller companies or perhaps unregistered. <br />
Here, we can see that Taxi Affiliation Services make up a huge chunk of the taxicab trips, a total of 25%, followed by Flash Cab of 11.8%. The other companies are generally smaller and make up single digit percentages of total trips. <br />
A short note is that some companies may potentially be affiliated with one another (such as Taxi Affiliation Services
and Taxi Affiliation Service Yellow). This chart showing the list of companies here can help us understand the current market share, and determine which are the more popular companies. <br />
More in-depth research on why these companies are perhaps preferred over others, etc, which can be useful. <br />
<br />

![image](https://user-images.githubusercontent.com/99934518/209704354-e04b42a9-f3a0-4108-904d-a1506f1645eb.png)

Now that we have taken a look at the general overview of taxi trips in Chicago, we can zone in onto the trends that can be derived from this dataset. <br />
One very crucial analysis can be derived from understanding the demand over a day. <br />
These are two charts here that shows the percentage of trips and the average fare across a day. <br />
The data is grouped based on the hours when the trip started. <br />
As seen from the first chart, the largest percentage of trips occurred at around 6-7pm, which is the peak hour after work hours. <br />
The lowest percentage of trips occurs at around 5AM, when there is likely the least activities and people are asleep. <br />
The second chart shows the average fare across the same timeframe. From this chart, it seems that the average fare sharply increases from 3am to a peak at 5am. <br /> Coincidentally, this is where the lowest percentage of trips happen. This may be attributed to a variety of factors, perhaps such as
longer trip distances (maybe to airports) or likely less drivers available at this timing. <br />
These two charts gives a general sense of when demand for the taxicabs are higher and what are the average fares earned from the trip at the associated
timing. This can potentially be used for pricing strategies and deployment of number of drivers at different timings, which is very useful. <br />
<br />

![image](https://user-images.githubusercontent.com/99934518/209705161-f10173da-f0c1-4182-964d-dd7b144c61dc.png)

Here, we can take a look at the general trend in the number of taxi cab rides over the years. <br />
As seen, there is a general declining trend from 2013 to the present date. The number of taxi trips has peaked in 2014 at a total of 37 million taxi trips, then generally declined until this year, 2022, where there are only about 6 million taxi trips. <br />
This is quite a sharp decline and taxi trips are generally becoming more scarce. <br />
A note is that that there is a seemingly sharp decline from 2019 to 2020, which is very likely due to covid-19, crippling travel in general, hence the sharp drop. It has since slowly recovered to 6 million in 2022. <br />
However, there is still a declining trend even before covid happened, and may be due to a plethora of factors (perhaps such as online cab services like UBER),
which is not recorded under taxi cabs in this dataset. <br />
Of course, this can signify something more, and businesses may have to pivot out of traditional taxi cabs if faced with a decreasing demand for these
cabs. <br />
<br />

![image](https://user-images.githubusercontent.com/99934518/209705392-682a7748-ef1e-45f3-a4a9-47419be95ffd.png)

As part of the trends, we can look into the different payment modes that the customers like to use for their taxi trips. <br />
In general, we are transitioning to being cashless in most parts of the world, and you would expect it to be the same in a rather developed state like Chicago. <br />
So, taking a look on the first chart, we can see the different payment modes across time. <br />
These values on the chart are the absolute values and not the relative percentages, but the purpose of this chart is to analyse the most popular payment methods. <br />
As evidently, cash and credit cards are the most popular payment methods, which will be further looked into in the second chart below. <br />
<br />

In the second part, as evidently, cash is becoming a less popular option, decreasing from 2013 to 2022, and credit card is becoming the majority payment option
as of 2022. <br /> 
However, a large portion of the customers still use cash. <br />
This can help us understand better the type of payment options that customers prefer. There is clearly a trend towards using
credit cards, but the cash option is not going away anytime soon, and the cabs should support these options. <br />

![image](https://user-images.githubusercontent.com/99934518/209705629-b5f39d66-d423-4d73-8546-10e41f382495.png)

Lastly, We can zone into the average fares and tips across time shown on the first chart. <br />
As seen from these charts, the fares and tips has been increasing across time. <br />
This can be due to factors such as inflation, increase in prices of petrol, increase in demand (not likely), increasing affluency of customers, etc. <br />
Again, it can be useful in pricing strategies , etc. <br />
<br />

Next, we can try to look for a correlation between fares and tips, as part of an investigation on their relationship. <br />
The size of the dots represent where the data is clustered. <br />
As seen, can have a general positive correlation, where higher average fares command a higher average tip too. <br />
Perhaps it can be used to calculate average total fare, estimate income and profits of taxi cabs, etc. <br />

## Areas of improvement and further analysis
1) More in-depth research into the trends and insights --> fares & tips, payment methods, etc <br />
2) Correlation & Causation --> confounding variables (e.g. supply of drivers in understanding demand) <br />
3) Tailoring to specific needs of the analysis from different viewpoints/stands (consumer, competitor, researcher, etc.) <br />
