# Bellabeat Case Study
## **Objective**
Bellabeat, a smart wearables company, wants to identify trends in smart device usage in order to inform its marketing strategy. This small company has an opportunity to gain more market share. In analyzing smart fitness data, we can observe how users are currently engaging with wearable technology and how their activity affects their health metrics. This will help Bellabeat see opportunities to target customers and potential customers for increasing engagement and customer base.

## Business Questions:
* What are some trends in smart device usage?
* How could these trends apply to Bellabeat customers?
* How could these trends help influence Bellabeat marketing strategy?

## Data Description 
The dataset contains users' FitBit data, identifying users by their identification number. According to Furberg, Briten et. al "Thirty eligible Fitbit users consented to the submission of personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring. Individual reports can be parsed by export session ID (column A) or timestamp (column B).  Variation between output represents use of different types of Fitbit trackers and individual tracking behaviors / preferences." 
I have cleaned the column names to eliminate the word "merged" from their title, and to put an underscore between the words, removing capitalization, for ease of querying. 
* **Calorie counts, represented in 3 tables**: Columns include the day/hour/minute time stamp, number of calories, and user ID
  * **daily_calories**
  * **hourly_calories**
  * **minute_calories**
* **daily_intensities**: Activity is broken down into columns referring to the level of intensity here, including minutes spent sedentary, lightly active, fairly active, and very active, and the distance traveled each day while at each intensity level,
* **hourly_intensity**: Total and average intensity per hour
* **Step counts, represented in 3 tables**: Columns include the day/hour/minute time stamp, number of steps, and user ID
* **minute_METs**: Metabolic Equivalent of Task per minute, with 1 being your resting metabolic rate. This number scale is a metric for intensity, which is represented by a name in other tables. According to Bailey, Dodd et. al:
    * Sedentary: Less than 1.5 METs (e.g., sitting, lying down, or sleeping)
    * Lightly Active: 1.5 to 3.0 METs (e.g., casual walking, doing dishes, or light housework)
    * Fairly Active: 3.0 to 6.0 METs (e.g., brisk walking, jogging, or mowing the lawn)
    * Very Active: Greater than 6.0 METs (e.g., running, jumping rope, or HIIT)
* **sleep_day**: gives total time in bed and total time asleep for comparison. I added a column with this ratio to show the difference each day comparing the time spent in bed vs. time spent asleep, and called it SleepEfficiency.
* **Duplicate Information**: daily_activities lists a lot of columns that are shared with the other daily calories, synthesized into one table. I was chose to lean on the table relevant to the metric for ease of understanding. When calculating steps, I used the daily_steps table/
  
## Insights
After analyzing the data, I observed the following trends:
* 72.72% of users log their sleep data
* Weight logs get little engagement from users
* Users are most active between 10am and 2pm on Saturdays and between 5pm and 7pm on weekdays, with less activity on Thursday and Friday.
* The most active hour per week is 1pm - 2pm on Saturday. 
* Users are more likely to be active in the afternoon and evening, with least activity in the morning.

## Business Recommendations
* Users clearly rely on metrics that are tracked automatically. Highlight the ease of getting personal metrics delivered in real time wihtout any need for manual input.
* To increase user engagement, focus on the known link between accountability and an active lifestyle. Include activity reminders on Thursdays and Fridays around 4pm and on Saturday around 10am. Advertise Bellabeat as a stylish accountability buddy. Additionally, encourage users to wear their Bellabeat to bed for accurate sleep data.
* Focus on the link between an active lifestyle and calorie burn without over-emphasizing weight logging, which seems to be of less interest to users based on low engagement.
* Regardless of lifestyle (mostly active or mostly sedentary), users who take more steps burn more calories. This provides the opportunity to market to both a fitness crowd and a fitness-skeptical crowd who are looking for small ways they can maintain a healthier lifestyle, such as increasing step count.
* Encourage users to wear their Bellabeat to sleep for up-to-date information on sleep and activity readiness.
* Offer an incentive for Bellabeat users to turn one year's worth of their anonymous data in order to gain a better picture of how user activity changes over time.

## Conclusion
Bellabeat has an opportunity to increase engagement with customers by sending targeted reminders to be active on days when users are statistically less likely to be active, such as Thursday and Friday, and by encouraging customers to wear their devices to sleep. Framing Bellabeat as a stylish partner for accountability will appeal to the fitness community. To grow its customer base, Bellabeat can appeal to the fitness skeptic who may be looking for a healthier lifestyle by highlighting how step tracking leads to calorie burn. This dataset is incomplete, with 30 users' data over only two months. For a more complete picture, Bellabeat should provide an incentive for users to consent to Bellabeat collecting at least a year's worth of data to better understand user engagement over time. This, along with a satisfaction survey after purchase, would give a more complete picture for future marketing strategies. 

## Citations

Bailey CP, Dodd KW, McClain JJ, Seo I, Wheeler W, Wolff-Hughes DL. Fitbit Physical Activity and Sleep Data in the All of Us Research Program: Data Exploration and Processing Considerations for Research. Med Sci Sports Exerc. 2025 Dec 1;57(12):2946-2953. doi: 10.1249/MSS.0000000000003804. Epub 2025 Jul 3. PMID: 40605186; PMCID: PMC12264798.

Furberg, R., Brinton, J., Keating, M., & Ortiz, A. (2016). Crowd-sourced Fitbit datasets 03.12.2016-05.12.2016 [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.53894](https://doi.org/10.5281/zenodo.53894)

