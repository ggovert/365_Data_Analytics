# Data_Analytics_Project

## Project 1: 365_Customer_Engagement_Data_Analytics
### Project Overview:
This project aims to provide insights into customer behavior at 365 Data Science. By analyzing various aspects of the customer behaviour data, we seek to gain a deeper understanding of customer behavior that impacted the company's performance

### Data Source:

All the dataset (txt file) that I used for this project is in the tableau_datasource folder. Containing all the needed data to make the customer behaviour dashboard

Data Definition:
- Engagement: The beginning of the lecture courses, quiz, or exam
- Onboarding: The first time engagement
- Student Type: Free-plan student or Paying student (monthly, quarterly, annually)

### Tools

- MySQL -Data Preparation, Analysis & Combining and Creating New Table
- Tableau - Creating Dashboard

### Data Preparation
In this phase, I used MySQL for the data preparation, and I performed the following tasks:
1. Data inspection
2. Handling missing values
3. Data cleaning and formatting

### Exploratory Data Analysis
EDA involved exploring the customer behavior data to answer key questions, such as:
- How Engaged are the students inside the platform, and how can this metric be improved?
- How long do students stay engaged on the  platform, and how can this period be extended?
- What's the difference in behavior between free and paid students?
- Which are the most popular courses on the platform
- How many students sit for an exam? 

### Data Analysis
Working with some interesting code/features in Mysql

```sql
SELECT a.student_id, b.date_engaged
CASE
WHEN x THEN y
END as paid
FROM table_a a LEFT JOIN table_b b USING (student_id);
```
After analyzing the data, I discovered that there are some duplicate data entries from the same student in the student_engagement table as a result of the free and paid subscriptions. I did this by using nested functions in SQL and ensuring that I only used the paid subscription as the beginning of engagement data.After that, i save this new data as csv with the name student_engagement.csv

### Creating Dashboard
Create 5 dashboards in total to analyze the data
[Tableau Dashboard](https://public.tableau.com/app/profile/giovanni.govert/viz/DataAnalysison365Platform/Overview?publish=yes) 

### Results/Findings
1. There was a significant increase in engagement from August to September 2022 when compared to the previous month. It is because of the marketing campaign that took place that month. We can conclude that the marketing campaign (the free days) was successful in increasing student engagement.
- Surprisingly, these increases in engagement are only visible for free students. There was no discernible increase in engagement among paid students.
2. According to the overall engagement data, there will be a 300% increase in student engagement between January and October 2022.
3. There was an increase in the percentage of people who registered and turned into students around September 2022. We conclude that the gamification strategy can increase the percentage of students who are onboarding.
4. The majority of free plan students are only engaged for the first month, after which their engagement drops dramatically. The majority of students, according to the hypothesis, cancelled their subscriptions before the 30-day period expired.
5. Paid students who stayed engaged throughout the year were the ones who paid annual subscriptions.
6. The average amount of time spent watching television by free plan students is around 20 minutes. This implies that the free student is interested in the unlock content provided by the 365 application to their free plan students.
7. It was difficult to predict the average number of minutes watched by paid students because each student has a different learning style. However, the average is around 540 minutes of content (roughly 2-3 extensive courses).

### Recommendation
1. Monthly retargeting to free plan student using paid ads to increase their engagement with the apps

### Limitation
The data only cover data from 1 January 2022 - 31 October 2022

### References
1. Udemy: Customer Behavior Analysis with SQL and Tableau

