# Bike Sharing
## Overview

Citi Bike is the nation's largest bike share program, with apporx 27,350 bikes and over 1,549 stations across Manhattan, Brooklyn, Queens etc. Based on the experience in New York city, an investor is ready to invest in Kate's idea to open a similar bike business in the of city of Des Moines.
For this purpose Kate analyze the New York city bike share data and presents following reports -
* 

## Results
A complete Story board have been generated in Tabuleau to walkthrough the details of analysis [Click Here](https://public.tableau.com/views/BikeSharingWorkbook/BikeSharingStory?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

To analyze the data the following steps have been followed
### 1) Convert the Tripduration 
Tripduration format in the given data file was in Numeric datatype. Inorder to covert the Numeric datatype to Datetime datatype we wrote code in Pandas.
Code file - [Jupyter Notebook File](NYC_CitiBike_Challenge.ipynb)

Below image shows comparison of the data format change
<p align="center"> <img src="Images/tripdurationComparison1.jpg.png"  align="center" height="400" width="700"></p>



Overall Data after the converted Tripduration
<p align="center"> <img src="Images/tripduration_aftermodification.png"  align="center" height="400" width="1000"></p>

### 2) Gender wise Bike rider breakdown
We can see from the below data that there are more Male bikers
<p align="center"> <img src="Images/Gender_Breakdown_percentage.jpg.png"  align="center" height="400" width="1000"></p>

### 3) Bike Utilization
This shows the Maximum utlization of Bikes and time in which it started the rides.
After converting the Tripduration to datatime instead of numeric , instead of Average of Triduration we are using Maximum of the Tripduration value.
<p align="center"> <img src="Images/Bike Utilization.jpg"  align="center" height="400" width="400"></p>

### 4) Starting and Ending Location
A quick comparison of Starting and Ending locations of bikers. 
It is pretty much same place.
<p align="center"> <img src="Images/Top Starting position.png"  align="center" height="350" width="450"> <img src="Images/Top Ending position.png"  align="center" height="350" width="450"></p>

### 5) Checkout times for User
The figure below shows the number of per hour of bike ride. A large proportions of trip lasted in less than an hour. Bikes are not used for long hours of durations.
<p align="center"> <img src="Images/Checkout times for Users.png"  align="center" height="400" width="1000"></p>

### 6) Checkout times by Gender
For most men and women, the average duration of biking is less than an hour.
<p align="center"> <img src="Images/Checkout Times by Gender.png"  align="center" height="400" width="1000"></p>

### 7) Trips per weekday per Hour
The figure shows that peak hours are morning 8am - 9am and evening 5pm - 7pm on most weekdays, Thursday evening looks to be most peak time.
During weekends day time gets busier compared to morning and evenings.
<p align="center"> <img src="Images/Trips by Weekday per Hour.png"  align="center" height="400" width="1000"></p>

### 8) Trips by gender and Weekday per hour
For both male and female riders, the demand for bike riding is high between morning 8am - 9am and evening 5pm to 6pm
<p align="center"> <img src="Images/Trips by Gender per Hour.png"  align="center" height="400" width="1000"></p>

### 9) Trips by Weekday and gender
-  Subscribers are more likely to use the bike share services.
-  Most subscibers are Male 
-  All the Unknowns are non - subscibers. which makes sense that their data is not stored in out database as they just come and use the services without subscribing.
<p align="center"> <img src="Images/User Trips by Gender by Weekday.png"  align="center" height="400" width="1000"></p>


## Summary
Based on the analysis we can conclude that
* Percentage of Male bikers is higher compared to Female and there is some part of Unknown who are non subscibers
* Most bikers used in Morning and Evening during weekdays. Day time usage is very less during weekdays compared to weekends.
* There is high % of subscribers , however, the non subscribers are also using the services which is a good too.
