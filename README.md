# Call Centre Trends Using PowerBI
Analysis of Call Centre Trends (A PWC Virtual Internship Project)- _Notebook By Jessica Addy_

# Introduction
PhoneNow, a fictitious call center, seeks openness and insight into the information gathered. They want to know how many calls were answered and how many were abandoned, as well as the speed with which they were responded, the duration of the calls, and overall customer satisfaction. They also want a dashboard with an accurate picture of long-term trends in consumer and agent behavior

# Contents
  1.  Project Objectives: Problem Statement
  2.  Data Sourcing
  3.  Data Cleaning
  4.  Findings and Recommendations
  
  
 # 1. Project Objectives
  The project seeks to identify
    •	Customer satisfaction in general
    •	Overall, how many calls were answered/abandoned
    •	Time-based calls
    •	Average call response time
    •	Average handling time (talk duration) versus calls answered -> agent performance quadrant
    

  # 2. Data Sourcing
  The data was provided by PWc as Task 2 of the virtual internship process.
  

  # 3. Data Cleaning
  Data cleaning was done in Power Query. 
    • To make the meaning of the data more obvious, the "Y" and "N" values for the Answered and Recovered Columns were changed to Yes and No, respectively.

• To extract the Weekday and Week Number from the Date, new columns were added to the data. These equations were employed:
  WeekDay = FORMAT (Sheet1[Date],"dddd")
  WeekDay Number = WEEKDAY (Sheet1[Date],2)
  This will aid in my analysis of the number of incoming calls received each day of the week so that I can determine which days had the most and fewest calls received. The Week Number made it easy for me to properly categorize my weeks' days such that Monday would be the first weekday and Sunday would be the last.
        
    • An column (Hour) was created from time column to help us analyze time-based calls. 
  
  ![Screenshot 2022-06-24 081443](https://user-images.githubusercontent.com/107724453/175509188-6d82a9d6-d023-421b-b23f-05b19490757c.png)
  
 # 4. Data Visualization
 
 
 # 5. Findings and Recommendations
 
 
 
 
  




  
  
