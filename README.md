# Call Centre Trends Using PowerBI
Analysis of Call Centre Trends (A PWC Virtual Internship Project)- By Jessica Addy_

# Introduction
PhoneNow, a fictitious call center, seeks openness and insight into the information gathered. They want to know how many calls were answered and how many were abandoned, as well as the speed with which they were responded, the duration of the calls, and overall customer satisfaction. They also want a dashboard with an accurate picture of long-term trends in consumer and agent behavior

# Contents
  1.  Project Objectives: Problem Statement
  2.  Data Sourcing
  3.  Data Cleaning
  4.  Dax Formulas and Data Visualization
  4.  Findings and Recommendations
  
  
 # 1. Project Objectives
  The project seeks to identify
  
    •Customer satisfaction in general
    •Overall, how many calls were answered/abandoned
    •Time-based calls
    •Average call response time
    •Average handling time (talk duration) versus calls answered -> agent performance quadrant
    

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
  
 # 4. DAX Functions and Data Visualization
 
 ## DAX Functions 
 These functions were applied to arrive at the data visualizations
  * Answered Calls = CALCULATE([Total Incoming calls], Sheet1[Answered (Y/N)]="Yes")
  * Unanswered Calls = CALCULATE([Total Incoming calls], Sheet1[Answered (Y/N)]="No")
  * Average SpeedTime = average(Sheet1[Speed of answer in seconds])
  * Average Time = AVERAGE(Sheet1[AvgTalkDuration])
  * ATD (Average Talk Duration) = format(AVERAGE(Sheet1[AvgTalkDuration]),"HH:MM:SS")
  * Averge CSAT Score = AVERAGE(Sheet1[Satisfaction rating])
  * Total Incoming calls = DISTINCTCOUNT(Sheet1[Call Id])
  * Unresolved = CALCULATE([Total Incoming calls], Sheet1[Resolved]="No")
  * Resolved = CALCULATE([Total Incoming calls], Sheet1[Resolved]="Yes")
 
 ## Dashboard
![CALL_CENTRER_TRENDS-1](https://user-images.githubusercontent.com/107724453/177151278-ac4eb41b-d290-4ec7-a652-abc184998779.png)

[Interact With Dashboard Here](https://app.powerbi.com/view?r=eyJrIjoiNDcyNTM5MTQtNGU3ZS00Njk0LWFkMWMtNGJjYWNjNTMwMDZkIiwidCI6ImU1MjBlNjgwLTk2OGMtNGM5Ny1hNjQ4LTc3ZjZmNmQ4MTA5ZiJ9)
 
 # 5. Findings and Recommendations
 
   PhoneNow recorded a total of 5000 inbound calls for the months and year under consideration (January–March 2021). All of our agents answered 81.1% of incoming calls, with Jim taking the majority of them. Every call that was received included complaints that were detailed and connected to different subjects, with a greater population being worried about streaming services. All concerns were resolved in 73.9% of cases. Jim made sure that the 485 incoming calls were answered.
   
   I also observed that the call center records the maximum number of phone calls throughout the workday at 5:00 pm, totaling 11.66 %, and the least at 6:00 pm, totaling 0.28 %. But we also see that the peak time for incoming calls is 5:00 pm on Mondays. The majority of these inbound calls occurred in March.

Prior to speaking with an agent, a consumer typically waits 67.52 seconds (1 minute and 8 seconds) on the phone. On a scale from 1 to 5, the standard of our services was rated as well, with an overall business grade of 3.40. Individually, Joe had a score of 3.3, while Martha received a 3.47.

Recommendation: 
  1. The agents and entire staff need to come to an understanding of what makes good customer experience
  2. Gain an understaning of system components, how and whom to contact so that they can be resolved
  3. Maintain the average reponse time to calls at 60-90seconds.
  4. Create systems that generate particualar customer experience.


## Thank you for taking time to read my Call Centre Analysis

[Interact with me here](https://twitter.com/addy_xls)


   
 
 
 


  
  
