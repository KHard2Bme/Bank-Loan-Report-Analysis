# Bank Loan Report Analysis     🏦                                      

## Table of Contents

- [Project Overview](#project-overview)
- [Requirements](#requirements)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Summary of Findings](#summary-of-findings)
- [Results from Findings](#results-from-findings)
  



## Project Overview
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



## Requirements
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
-----

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
-----

DASHBOARD 3: DETAILS

In our Bank Loan Report project, we recognize the need for a comprehensive 'Details Dashboard' that provides a consolidated view of all the essential information within our loan data. This Details Dashboard aims to offer a holistic snapshot of key loan-related metrics and data points, enabling users to access critical information efficiently.
- Objective:
The primary objective of the Details Dashboard is to provide a comprehensive and user-friendly interface for accessing vital loan data. It will serve as a one-stop solution for users seeking detailed insights into our loan portfolio, borrower profiles, and loan performance.

---

FILTERS :

- State
- Grade
- Purpose

---


Stakeholder Request: 

- The Marketing Director would like to know detailed customer insights which will help in her marketing strategies to specific customer segments (attract those with very favorable risk profiles).



## Data Sources
---
The primary dataset used for this analysis is the "Financial_loan.csv" file obtained from Kaggle which contains 38,576 rows and 24 columns.


## Tools
---
- <b>pandas, numpy, datetime, matplotlib, seaborn.</b> 
- <b>Microsoft Excel</b>



I will be using python to clean, process, and analyze the dataset (detailed steps will be shown within the Jupyter Notebook).<br>

The <b>Bank Loan Analysis(Verification of Report ).ipynb</b> notebook will be used to confirm numeric outcome from each Dashboard field.<br>

I will be using <b>Excel</b> to create reports and automated dashboard ( reports and dashboard provided in Bankloan_data.csv file).<br>

      

## Exploratory Data Analysis
---
>note:  Questions 1 through 6 are answered in Bank Loan Analysis( Verification of Report ).ipnb notebook.

>note:  Questions 7 through 15 are answered in Bank Loan Analysis.ipnb notebook.



Questions the client has that can now be answered:

1. What is the total amount, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

2. What is the total funded amount, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

3. What is the total amount received, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

4. What is the average interest rate, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

5. What is the average DTI, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

6. What is the total good and bad loan applications issued, funded amounts, and amounts received?

7. What is the distribution of loans by risk classification?

8. We know that the risk classification assigned to a loan represents a customers creditworthiness; higher grades signify lower risk. How do loans assigned a grade of A and B differ from all the others?

9. Within risk classification A, which loan purpose has the largest amount of applicants, and which has the least?

10. Within risk classification A, which loan purpose has the lowest and highest interest rates within this category?

11. Within risk classification A, there are loans with a 36 and 60 month fixed rate. What is the distribution of loans within each and their differences by interest rate?

12. Within risk classification A, which home ownership group has the most applications submitted? Which has the lowest interest rate for a 36 and 60 month term loan?

13. What states have applicants who pay a mortgage and have the lowest interest rate and DTI Ratio?

14. What states have applicants who pay rent and have the lowest interest rate and DTI Ratio?

15. What states have applicants who own property and have the lowest interest rate and DTI Ratio?


## Summary of Findings
### Question #1: 
What is the total amount, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

![1](https://github.com/user-attachments/assets/aa4da9c9-5149-43b4-b819-933424474ec9)
![1a](https://github.com/user-attachments/assets/1eb469ba-b87b-48bf-9b18-2a6210d6b532)
![1b](https://github.com/user-attachments/assets/f4dbb757-8523-49ff-b067-a7062de87333)


### Question #2:

What is the total funded amount, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?
![2](https://github.com/user-attachments/assets/bd4ac3cb-5fe7-48ad-8ea9-285d687aeb4d)
![2a](https://github.com/user-attachments/assets/dca6364c-59d5-45de-a0a3-ba9acdb3d1d6)
![2b](https://github.com/user-attachments/assets/d6c99e3f-3f79-402c-a80e-7af9dd9dcfca)

### Question #3: 
What is the total amount received, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?
![3](https://github.com/user-attachments/assets/bef4f108-b3ac-4e72-9e01-2b2b531096b4)
![3a](https://github.com/user-attachments/assets/49568b6b-49de-43c6-a794-844de54ed4d9)
![3b](https://github.com/user-attachments/assets/16f594bc-4195-4f90-bf04-eb68b03aab4a)

### Question #4: 
What is the average interest rate, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?
![4](https://github.com/user-attachments/assets/e2dee734-7ffb-435f-8dd6-efb2bb32a858)
![4a](https://github.com/user-attachments/assets/6ca0eed8-0307-46c4-ad75-5f3034528576)
![4b](https://github.com/user-attachments/assets/6951ca1a-85c7-4179-9587-2e7ff0316c3b)

### Question #5: 
What is the average DTI, Month-To-Date (MTD), and Previous-Month-To-Date (PMTD) of loan applications?

![5](https://github.com/user-attachments/assets/9dbf33d4-05cb-424d-945a-b1411d23c1ba)

![5a](https://github.com/user-attachments/assets/cd6c4b2d-6d85-4eac-90cb-c13867404e81)

![5b](https://github.com/user-attachments/assets/e3a042f4-4ae7-493d-a415-b4ab5baa9471)


### Question #6: 
What is the total good and bad loan applications issued, funded amounts, and amounts received?
![6](https://github.com/user-attachments/assets/1e4bcc61-b641-4708-9123-285cbf64cedf)
![6a](https://github.com/user-attachments/assets/5ce7cf05-eeff-4c09-98af-2c17aae32466)
![6b](https://github.com/user-attachments/assets/e72ab6ef-b12b-40ad-b876-5f44e9723144)
![6c](https://github.com/user-attachments/assets/a4508d70-216b-4c9e-af58-045aab22cbc3)
![6d](https://github.com/user-attachments/assets/155d1c24-a0fe-4453-9018-a70490869115)

### Question #7: 
What is the distribution of loans by risk classification?

### Question #8:
 We know that the risk classification assigned to a loan represents a customers creditworthiness; higher grades signify lower risk.
 How do loans assigned a grade of A and B differ from all the others?

### Question #9:
Within risk classification A, which loan purpose has the largest amount of applicants, and which has the least?

### Question #10: 
Within risk classification A, which loan purpose has the lowest and highest interest rates within this category?

### Question #11: 
Within risk classification A, there are loans with a 36 and 60 month fixed rate. 
What is the distribution of loans within each and their differences by interest rate?

### Question #12:
Within risk classification A, which home ownership group has the most applications submitted?
Which has the lowest interest rate for a 36 and 60 month term loan?

### Question #13:
 What states have applicants who pay a mortgage and have the lowest interest rate and DTI Ratio?
 
### Question #14:
 What states have applicants who pay rent and have the lowest interest rate and DTI Ratio?
 
### Question #15:
What states have applicants who own property and have the lowest interest rate and DTI Ratio?



## Results from Findings
---

Stakeholder Request:

	The Marketing Director would like to know detailed customer insights which will help in her marketing strategies to specific customer segments (attract those with very favorable risk profiles).

What are a few customer insights from the dataset of applicants who have a mortgage, rent as well as own property?


### Those applicants who have a Mortgage:
- the average employment length is about 6 years
- the employee titles vary within the financial, healthcare, insurance, and manufacturing service sectors
- all loans have a 36 month term
- the average annual salary is about $ 73,419.37
- the average DTI ratio is 0.03 percent
- the interest rate is 0.05 percent 
- the average loan amount is $ 7,806.94
- the loan type has a risk classification of A
- the loan purpose is debt consolidation
- the loan status is fully paid
- the applicants reside in 13 states


### Those applicants who rent :
- the average employment length is about 5 years
- the employee titles vary within the Financial, Technology, State agency service sectors
- all loans have a 36 month term
- the average annual salary is about $ 92,855.56
- the average DTI ratio is 0.04 percent
- the interest rate is 0.05 percent 
- the average loan amount is $7,155.56
- the loan type has a risk classification of A
- the loan purpose is debt consolidation
- the loan status is fully paid
- the applicants reside in 7 states

### Those applicants who own property :
- the average employment length is about 5.5 years
- the employee titles are in the Orthodontics manufacturing and healthcare technology services
- all loans have a 36 month term
- the average annual salary is about $69,998.00
- the average DTI ratio is 0.03 percent
- the interest rate is 0.05 percent 
- the average loan amount is $6,900.00
- the loan type has a risk classification of A
- the loan purpose is debt consolidation
- the loan status is fully paid
- the applicants reside 2 states


