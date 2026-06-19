# Bellabeat Case Study
## **Objective**
Bellabeat, a smart wearables company, wants to identify trends in smart device usage in order to inform its marketing strategy. 

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
* **daily_intensities**: Activity is broken down into columns referring to the level of intensity here, including minutes spent sedentary, lightly active, fairly active, and very active, and the distance traveled each day while at each intensity level
* **hourly_intensity**: Total and average intensity per hour
* **Step counts, represented in 3 tables**: Columns include the day/hour/minute time stamp, number of steps, and user ID
* **minute_METs**: Metabolic Equivalent of Task per minute, with 1 being your resting metabolic rate. This number scale is a metric for intensity, which is represented by a name in other tables. According to Bailey, Dodd et. al:
    * Sedentary: Less than 1.5 METs (e.g., sitting, lying down, or sleeping)
    * Lightly Active: 1.5 to 3.0 METs (e.g., casual walking, doing dishes, or light housework)
    * Fairly Active: 3.0 to 6.0 METs (e.g., brisk walking, jogging, or mowing the lawn)
    * Very Active: Greater than 6.0 METs (e.g., running, jumping rope, or HIIT)

## Citations

Bailey CP, Dodd KW, McClain JJ, Seo I, Wheeler W, Wolff-Hughes DL. Fitbit Physical Activity and Sleep Data in the All of Us Research Program: Data Exploration and Processing Considerations for Research. Med Sci Sports Exerc. 2025 Dec 1;57(12):2946-2953. doi: 10.1249/MSS.0000000000003804. Epub 2025 Jul 3. PMID: 40605186; PMCID: PMC12264798.

Furberg, R., Brinton, J., Keating, M., & Ortiz, A. (2016). Crowd-sourced Fitbit datasets 03.12.2016-05.12.2016 [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.53894](https://doi.org/10.5281/zenodo.53894)

