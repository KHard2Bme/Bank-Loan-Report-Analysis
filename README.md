# Bank Loan Report Analysis     🏦                                      

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

Bank Loan Analysis  
---
    
In order to monitor and assess the bank's lending activities and performance, we need to create a comprehensive Bank loan report using Microsoft Excel.
    
This report aims at providing insights into key loan-related metrics and their changes over time.

The report will help us make data-driven decisions, track our loan portfolio's health, and identify trends that can inform our lending strategies.

Before we can do this, we must first take a look at the data using Python; data cleaning, wrangling, EDA (Exploratory Data Analysis), and visualization.

Once completed we will export the dataset as a .csv file and import into Microsoft Excel for report and dashboard creation; see below figures A, B, and C.

<b>Figure A<b>
![summary](https://github.com/KHard2Bme/US_Call_Center_Dashboard_Excel/assets/146769989/878e7299-f50b-4a47-aa4a-10a7f88166cc)

<b>Figure B<b>
![chicago](https://github.com/KHard2Bme/US_Call_Center_Dashboard_Excel/assets/146769989/62d2a442-04b0-44d8-aca4-8a6c432e8d2e)


<b>Figure C<b>
![chicago](https://github.com/KHard2Bme/US_Call_Center_Dashboard_Excel/assets/146769989/62d2a442-04b0-44d8-aca4-8a6c432e8d2e)



### Requirements
---

Client wants to have an automated dashboard for year 2021 so that they can gather customer insights from the below requirements ( 3 Dashboards created ):


DASHBOARD 1: SUMMARY

- Primary KPI:
1. Total Loan Applications (in addition to showing Month-to-Date (MTD) Loan Applications and Month-over-Month (MoM) changes).
2. Total Funded Amount (in addition to showing Month-to-Date (MTD) Total Funded Amount and Month-over-Month (MoM) changes).
3. Total Amount Received (in addition to showing Month-to-Date (MTD) Total Amount Received and Month-over-Month (MoM) changes).
4. Average Interest Rate (in addition to showing Month-to-Date (MTD) Total average interest rate and Month-over-Month (MoM) changes).
5. Average Debt-to-Income Ratio (DTI) (in addition to showing  Month-to-Date (MTD) Debt-to-Income and Month-over-Month (MoM) changes).


- Good Loan v Bad Loan KPI’s:
 
Good Loan KPIs ( loans with status of 'Fully Paid' and 'Current'):
1.	Good Loan Application Percentage
2.  Good Loan Applications
2.	Good Loan Funded Amount
3.	Good Loan Total Received Amount

- Bad Loan KPIs ( loans with a status of 'Charged off'):
1.	Bad Loan Application Percentage
2.	Bad Loan Applications
3.	Bad Loan Funded Amount 
4.	Bad Loan Total Received Amount

- Loan Status Breakdown KPI's:
1. Loan Applications
2. Loan Funded Amount
3. Loan Amount Received
4. Loan Interest Rate
5. Loan DTI Ratio

DASHBOARD 2: OVERVIEW

1. Monthly Trends by Issue Date (Line Chart):
- Chart Type: Line Chart
- Objective: This line chart will showcase how submitted loan Applications vary over time, allowing us to identify seasonality and long-term trends in lending activities.

2. Regional Analysis by State (Filled Map):
- Chart Type: Filled Map
- Geographic Regions: States
- Objective: This filled map will visually represent lending metrics categorized by state, enabling us to identify regions with significant lending activity and assess regional disparities.

3. Loan Term Analysis (Donut Chart):
- Chart Type: Donut Chart
- Segments: Loan Terms (e.g., 36 months, 60 months)
- Objective: This donut chart will depict loan statistics based on different loan terms, allowing us to understand the distribution of loans across various term lengths.

4. Employee Length Analysis (Bar Chart):
- Chart Type: Bar Chart
- X-Axis: Employee Length Categories (e.g., 1 year, 5 years, 10+ years)
- Y-Axis: Metrics' Values
- Objective: This bar chart will illustrate how lending metrics are distributed among borrowers with different employment lengths, helping us assess the impact of employment history on loan applications.

5. Loan Purpose Breakdown (Bar Chart):
- Chart Type: Bar Chart
- Objective: This bar chart will provide a visual breakdown of loan metrics based on the stated purposes of loans, aiding in the understanding of the primary reasons borrowers seek financing.

6. Home Ownership Analysis (Tree Map):
- Chart Type: Tree Map
- Objective: This tree map will display loan metrics categorized by different home ownership statuses, allowing for a hierarchical view of how home ownership impacts loan applications and disbursements.

DASHBOARD 3: DETAILS

In our Bank Loan Report project, we recognize the need for a comprehensive 'Details Dashboard' that provides a consolidated view of all the essential information within our loan data. This Details Dashboard aims to offer a holistic snapshot of key loan-related metrics and data points, enabling users to access critical information efficiently.
- Objective:
The primary objective of the Details Dashboard is to provide a comprehensive and user-friendly interface for accessing vital loan data. It will serve as a one-stop solution for users seeking detailed insights into our loan portfolio, borrower profiles, and loan performance.

FILTERS :

- State
- Grade
- Purpose




Stakeholder Request: 

- The Marketing Director would like to know detailed customer insights which will help in her marketing strategies to specific customer segments (attract those with very favorable risk profiles).



### Data Sources
---
The primary dataset used for this analysis is the "Financial_loan.csv" file obtained from Kaggle which contains 38,576 rows and 24 columns.


### Tools
---
- <b>pandas, numpy, datetime, matplotlib, seaborn.</b> 
- <b>Microsoft Excel</b>



I will be using python to clean, process, and analyze the dataset (detailed steps will be shown within the Jupyter Notebook).<br>

The <b>Bank Loan Analysis(Verification of Report ).ipynb</b> notebook will be used to confirm numeric outcome from each Dashboard field.<br>

I will be using <b>Excel</b> to create reports and automated dashboard ( reports and dashboard provided in Bankloan_data.csv file).<br>

      

### Exploratory Data Analysis
---
Questions the client has that can now be answered.

1. What is the total amount of loan, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) applications?

2. What is the total funded amount of loan, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) applications?

3. What is the total amount received of loan, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) applications?

4. What is the average interest rate of loan, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) applications?

5. What is the average DTI of loan, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) applications?

6. What is the total good and bad loan applications issued? funded amounts, and amounts received?

7. We know that the risk classification assigned to a loan represents a customers creditworthiness; higher grades signify lower risk.
   How do loans assigned with a grade of A differ from all the other loans?

8. Within risk classification A, which loan purpose has the largest amount of applications submitted?

9. Within risk classification A, there are loans with a 36 month and 60 month term. What is the distribution of loans by term and is there a difference by interest rate?

10. Within risk classification A, which home ownership group has the most applications submitted? Which has the lowest interest rate by 36 and 60 month term?

11. Within risk classification A, What are the states each creditor resides in? Which states have the largest percentage of applicants, and out of these which has the lowest interest rate on loans based off those who rent, own a home and own property? 





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


