# bellabeat
Built-in R studio for Google Capstone project (Case Study 2)

You are a junior data analyst on the marketing analyst team at Bellabeat, a high-tech manufacturer of health-focused products for women. Bellabeat is a successful small company, but they have the potential to become a larger player in the global smart device market. Urška Sršen, cofounder and Chief Creative Officer of Bellabeat believes that analyzing smart device fitness data could help unlock new growth opportunities for the company. You have been asked to focus on one of Bellabeat’s products and analyze smart device data to gain insight into how consumers are using their smart devices. The insights you discover will then help guide the marketing strategy for the company. You will present your analysis to the Bellabeat executive team and your high-level recommendations for Bellabeat’s marketing strategy.

I have used the steps from the ask, prepare, process, analyze, share, and act to create a roadmap and analyze the Case Study.
# ASK- <br>
Identify trends in how consumers use non-Bellabeat smart devices to apply insights into Bellabeat’s marketing strategy. Got to know about the stakeholders.
# PREPARE- <br>
Fitbit Fitness Tracker Data, which is open source and made publicly available, was obtained from Kaggle and used as the data source for our case study. The submission of personal tracker data, including minute-level output for physical activity, heart rate, and sleep tracking, was approved by thirty qualified Fitbit users. Since each row represents a single time point for each subject, the data is regarded as long, hence, each subject will have data in several rows. We may run into sampling bias because of the small sample size (30 users) and the lack of demographic data, such as age or gender. The sample's representativeness of the entire population is uncertain. We would also get into the issue of the dataset not being up to date.
# PROCESS- <br>
Because of accessibility, the volume of data I will be working with, and the ability to build data visualizations to share my findings and suggestions with stakeholders, I have decided to do my study using R.
# ANALYZE- <br>
I analyzed the trends of the users of FitBit and determined if that could help me with BellaBeat’s marketing strategy. Started by installing all the required packages, then importing the data using read_csv. After viewing the data sets, I removed the NA and duplicate values, after which only 3 entries were left in the weight dataset therefore I decided to discard that set from the analysis. Then I made all column names in a similar format to merge the datasets later on, similarly setting the date/time columns in the same format. Finally merged daily activity and sleep data, which will be used later on for analysis.
# SHARE- <br>
## 1. Summary of daily activity:
<img width="744" alt="Screenshot 2025-02-14 at 2 29 32 PM" src="https://github.com/user-attachments/assets/3e69342f-f77f-4dae-8ed2-33538bc5e3c0" />

## 2. Steps taken vs. calories burned
 <img width="800" alt="Screenshot 2025-02-14 at 11 46 25 AM" src="https://github.com/user-attachments/assets/eb76bfea-db89-40e6-b419-a76b0b52acf2" />

 ### Conclusion- <br>
A positive correlation between the total steps taken and the amount of calories burned is observed.

## 3. Daily Steps taken
<img width="961" alt="Screenshot 2025-02-14 at 12 23 16 PM" src="https://github.com/user-attachments/assets/7e128d56-b0cf-4ae4-9fe2-6f14400b6c88" />

### Conclusion- <br>
Users are most likely to achieve the target step goal of 7500 steps almost everyday, especially on Monday, Tuesday, Wednesday, and Saturday, except Sunday.

## 4. Sleep time
   <img width="1120" alt="Screenshot 2025-02-14 at 12 45 03 PM" src="https://github.com/user-attachments/assets/ef4bcadf-c946-423c-be0c-e44e9254720f" />

### Conclusion- <br>
Users are not getting sufficient sleep time of 8 hours.

## 5. Hourly steps during the day
   <img width="1288" alt="Screenshot 2025-02-14 at 1 07 53 PM" src="https://github.com/user-attachments/assets/5e1bb79d-f0eb-4f35-bec3-249cf13af292" />

### Conclusion- <br>
1. Users are the most active from 8 am to 7 pm.
2. Most of the activity happens between 5 pm to 7 pm, maybe this is the time they commute from work, head to the gym, go for a walk, or simply go out.
3. The period from 5 pm to 7 pm can be used to alert the users to perform some activity like walking or jogging using the Bellabeat app.

## 6. How long does a person use the product
   <img width="1001" alt="Screenshot 2025-02-14 at 1 24 46 PM" src="https://github.com/user-attachments/assets/01e398b7-126e-49ec-8ce5-62e341fd14cd" />
   
### Conclusion- <br>
1. 50% of the users use their device frequently, between 21 to 31 days.
2. 12% are moderate users who use their device between 11 to 20 days.
3. 38% of users rarely use their device.

# ACT- <br>
Bellabeat was founded to empower women by giving them access to information about their behaviors and health.
I will react to the business task of assisting Bellabeat with its marketing strategy based on my findings after evaluating the Fitbit Fitness data as we know that our main target is young and adult women.

Since the datasets used have a small sample size and may be skewed due to the lack of user demographic information, I would suggest using tracking data from Bellabeat's device for additional study.

Recommendation-
1. Daily alerts on steps taken should be sent to the user.
2. Daily notification on sleep, to have at least 8 hours of sleep.
3. Daily calorie consumption alerts according to their customisation.
4. A reward system should be established in return for goals achieved, like the step count or 8 hours of sleep. This will keep the audience engaged and motivated to use the device more.
