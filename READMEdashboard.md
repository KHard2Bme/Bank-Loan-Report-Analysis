# US_Call_Center_Dashboard      📲                                        

## Table of Contents

- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Summary of Findings](#summary-of-findings)
- [Results from Findings](#results-from-findings)
- [Recommendations](#recommendations)



### Project Overview
---

This data analysis project aims to provide insights into the performance of each call center over a one year period; Sept 1, 2020 through Sept 31, 2020 .</b> 

By analyzing various aspects of the data, I seek to identify trends, make data-driven recommendations, and gain a deeper understanding of the company's performance.</b> 

I will also perform Exploratory Data Analysis on the dataset to answer a few questions derived along the way.</b>




### Requirements
---
![summary](https://github.com/KHard2Bme/US_Call_Center_Dashboard_Excel/assets/146769989/878e7299-f50b-4a47-aa4a-10a7f88166cc)
![chicago](https://github.com/KHard2Bme/US_Call_Center_Dashboard_Excel/assets/146769989/62d2a442-04b0-44d8-aca4-8a6c432e8d2e)



Client wants to have an automated dashboard for year 2020 so that they can have insight on the below requirements:

- Primary KPI:

         a.) Total calls to Call Centers

         b.) Total calls by channel:
             - Call center  
             - Chatbot  
             - Email
             - Web

              
- Secondary KPI:  

              a.) Report showing calls by call center  
              b.) Report showing calls by sentiment.  
              c.) Column chart showing reason by sentiment.  
              d.) Column chart showing response time by call center. 
              e.) Chart showing total count by reason of call
              f.) Grid view dashboard allowing stakeholders to search for granular information in dataset and  download if needed.

- Filters:

              a.) Call day
              b.) Call center
              c.) Weekday or Weekend
              d.) Sentiment
              e.) Reason    

### Data Sources
---

Call Center Data: The primary dataset used for this analysis is the "Call_Center.csv" file obtained from Kaggle which contains fictitious data.


### Tools
---
- <b>pandas, numpy, matplotlib, seaborn.</b> 
- <b>Microsoft Excel</b>



I will be using python to clean, process, and analyze the dataset (detailed steps will be shown within the Jupyter Notebook).

I will be using Excel to create reports and automated dashboard ( reports and dashboard provided in Call_Center.csv file).

      

### Exploratory Data Analysis
---
Questions the client has that can now be answered.
1. What is the total number of calls received by call center? How many calls were received by each call center and percentage? weekday and weekend?</b>
2. What is the total number of calls received by each channel?</b>
3. Which day of the month received the most calls? The least?</b>
4. Which day of the month received the most negatively ranked calls? Calls ranked as very negative?</b>
5. Of the negatively ranked calls on Sept. 10, which call center received the most calls?</b>
6. Of the very negative ranked calls on Sept. 17, which call center received the most calls?</b>
7. How many total calls are in the Billing Question category? How many billing questions make up the negative and very negative categories?</b>
8. How many total calls are ranked as negative and very negative? How many negative and very negative calls were received by the Los Angeles/CA call center?</b>
9. What is the total number of calls categorized as below SLA, and how many were received by the Los Angeles/CA call center?</b>
10. Which state has the most calls ranked negative, and what are the top 2 cities? Which state has the most calls ranked very negative, amd what are the top 2 cities?</b>


## Summary of Findings

Question #1: 
What is the total number of calls received by call center?
How many calls were received by each call center and percentage? weekday and weekend?

Question #2: 
What is the total number of calls received by each channel?

Question #3: 
Which day of the month received the most calls? The least?

Question #4: 
Which day of the month received the most negatively ranked calls? Calls ranked as very negative?

Question #5: 
Of the negatively ranked calls on Sept. 10, which call center received the most calls?

Question #6: 
Of the very negative ranked calls on Sept. 17, which call center received the most calls?

Question #7: 
How many total calls are in the Billing Question category?
How many billing questions make up the negative and very negative categories?

Question #8: 
How many total calls are ranked as negative and very negative?
How many negative and very negative calls were received by the Los Angeles/CA call center?

Question #9: 
What is the total number of calls categorized as below SLA, and how many were received by the Los Angeles/CA call center?

Question #10: 
Which state has the most calls ranked negative, and what are the top 2 cities?
Which state has the most calls ranked very negative, amd what are the top 2 cities?




### Results from Findings
---

The analysis results are summarized as follows:

1.  A large percentage of inbound calls fall within the negative sentiment category, making up roughly 34% of total calls. Of those calls 71% fall within the billing questions reason type, followed by 14% in payments.  
  This is also true within every call center, having a large percentage of the calls falling within the negative sentiment category as well.

2.  Regarding call response time, a large percentage of the total inbound calls fall within the SLA; 63%, but 25% of the calls are below the SLA.
  
3. There seems to be a correlation between calls that have a negative sentiment and those falling below the SLA. Most of the calls come in through the call center channel on weekdays, and the reason type is either billing questions or payment. This is the case for all call centers.

### Recommendations
---

Based on the analysis, we recommend the following actions:

In order to find out the exact issue at hand we will need to first retrieve the audio recordings of each agent who picked up a call at designated call time stamp. We need to listen to each call and determine.

   - was call picked up and placed in queue
   - how long was the customer waiting in queue/did they hang up while waiting
   - did the agent answer all questions correctly and appropriately
   - was the customer satisfied with answer, if not what were next steps
   - was customer transferred to another Department or Manager for assistance and did that call go through successfully
   - were questions answered after being transferred.

Once we gather enough data, research the findings and try to understand the trends we can then come to a conclusion as to what the root cause or causes are.


