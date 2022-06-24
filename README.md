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
    • The "Y" and "N" values for both Answered and Recovered Column was replaced with Yes  and No respectively to communicate clearly what the data represents.

    • New Colums were added to the data to extract the Weekday and Week Number from the Date. These formulas were used:
        Week day = FORMAT(Sheet1[Date],"dddd")
        WeekDay = WEEKDAY(Sheet1[Date],2)
    The purpose if this is to help me analyze the number of incoming calls during the week and make deductions on which days recorded the most and least number of calls. The Week Number helped me clearly custom sort my weeks days to represent Monday as the first day of the weeks and Sunday as the last
        
    • An column (Hour) was created from time column to help us analyze time-based calls. 
  
  
 # 4. Data Visualization
 
 
 # 5. Findings and Recommendations
 
 
 
 
  




  
  
