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
After analyzing the data, I discovered that there are some duplicate data entries from the same student in the student_engagement table as a result of the free and paid subscriptions. I did this by using nested functions in SQL and ensuring that I only used the paid subscription as the beginning of engagement data.After that i save this new data as csv with the name student_engagement.csv

### Results/Findings
Tableau Dashboard:[Dashboard] (https://public.tableau.com/app/profile/giovanni.govert/viz/DataAnalysison365Platform/Overview?publish=yes) 

### Recommendation

### References
1. Udemy: Customer Behavior Analysis with SQL and Tableau

