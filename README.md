# Chickago Bike Sharing System (Part 2)

## Exploring Visualization
Creating an awareness of who is using Divvy bikes, leads to insights on how the service meets customer needs. Analysis like this can 
provide operational insights for balancing product availability, as well as showing seasonal variances. It can also become fuel for 
finding opportunities to increase customer satisfaction and engagement.</br>
In the data from the trips table, there are several fields that could bring insight in to who is making the most of the Divvy bike 
service. The fields that are of interest to us are **usertype, gender,** and **birthyear**. here are two general groups that use the 
Divvy bike service: **subscribers**, who are likely to be commuters, and **non-subscribers**, called **customers**, who are often 
tourists. 
More personal information is shared by riders with Divvy when a subscription service is purchased. As a result, the dataset contains 
their **gender** and **birthyear**. For the non-subscribers, in the absence of that ongoing relationship, those fields do not contain 
data and are reflected as null values in the dataset. Note that it's possible for subscribers to cancel their subscription and become 
customers. In that case, the Gender and Birthyear information will be kept, meaning that some customers will have values for these 
fields.</br>
Because we know the reason behind the **missing information**, we can easily **retitle** those labels within Tableau and increase the 
available insights from the data.</br>
Let's replace the **Null values** with the label **Day Pass Riders**, indicating that these users don't have an ongoing relationship 
with Divvy and just rented a bike for one day.

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/1_Users_Divvy.JPG "Logo Title Text 1")

**Male subscribers** have used the Divvy bikes for a total of **906,649 trips**. That's more than double the amount of 
**any of the other groups**. This information could come in handy when setting up a **marketing campaign**.</br>
The visualization was enhanced by adding filters that reflect only the rides that actually happened between specific locations or 
occurred in a specific window of time.</br>
**How many Divvy Day Pass Riders started and ended at Chicago's Adler Planetarium during the month of June 2019?**

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/2_Users_Divvy.JPG "Logo Title Text 1")

The Answer is **255**. Notice how we can uncover **valuable insights** by adding **filters** to this visualization. Drilling down 
like this can help us make better decisions regarding the amount of **Divvy bikes** available at the **Adler Planetarium** 
during **summer months**.

## KPI Dashboard
A key performance Indicator (KPI) is a measurable value that tracks a company’s key business objectives. A **KPI dashboard** has been 
created for the users of **Divvy bikes** to highlight the usage of the bikes with some filtering options such as **month, Year, 
from station, to station,** and **gender**. The **KPI Dashboard** holds only two worksheets. One of them has already been created 
above and next one is the following one.

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/3_Users_KPI.JPG "Logo Title Text 1")

Here, right side in picture filter options is available to filter out data.</br>
Now, by adding both visualizations just created, a dashboard has been generated. Creating an interactive relationship between the 
**KPI chart** and the **bar chart** describing the customers of **Divvy Bikes** can open **new doors for insights**.</br>

**What number shows up in the KPI chart when you select the bar related to female Subscribers in January 2019?**</br>

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/4_KPI_Dashboard.JPG "Logo Title Text 1")

The answer is **18550**. The visualizations in the dashboard automatically filters based on the selections.</br>

The dashboard was enhanced by adding more filters based on the calculated fields that were created in Part 1. These help one further 
evaluate the data. Earlier, the riders who were starting and ending at Adler Planetarium during a specific time of year were 
considered. Here, it was discovered that how many riders started this trip during the morning on a weekend throughout the six months 
of trips recorded in this dataset.</br>

**How many total rides that started and ended at Adler Planetarium occurred during the morning on a weekend?**</br>
The answer is **36** (See the following picture)

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/5_KPI_Dashboard.JPG "Logo Title Text 1")

**Of the two user types, Customer and Subscriber, which type of user did the majority of these rides?**
The answer is **Customer**.</br>
That makes sense, since most customers are tourists. Subscribers are more likely to be commuters and won't need the bike during 
the weekend.

## Visualizing Age Distribution
From **Birthyear** field calculate the users' age can be easily calculated. **Age** is another demographic element that 
**impacts businesses**. A company's products and services are more likely to appeal to certain **age groups**. If we know which 
**users** are using **Divvy bikes** more than others, we can set up successful **marketing campaigns targeting these users**.</br>

For **Divvy** to serve its **customers** or **potential customers** in a way that meets their needs well, it is important to understand 
what the age distribution looks like. A histogram is the perfect visualization for this. Before that, age calculation was done using 
calculated field.</br>

After filtering out the ages less than 16, greater than 90 and NULLs the following bar chart is presented

![alt text](https://github.com/asifsamy/chickago-bike-sharing-02/blob/master/images/6_Userr_Age.JPG "Logo Title Text 1")

**How many trips were taken by 27-year-old Subscribers?**</br>
The answer as **71,853 subscribers**. Looking at the histogram, it seems like most **Divvy users** are in their **twenties** or 
**thirties**.

