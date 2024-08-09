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

I will be using <b>Excel</b> to create reports and automated dashboard ( reports and dashboard provided in Bankloan_data.xlsx file).<br>

      

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

![7](https://github.com/user-attachments/assets/a6623757-a0c5-4f7c-9b98-66785d66127e)
![7a](https://github.com/user-attachments/assets/e26e104b-d8f5-4f4e-96b2-3c921631b966)
![7b](https://github.com/user-attachments/assets/fb1a6511-de3d-4ac8-8e18-d4b827d42508)
![7c](https://github.com/user-attachments/assets/29536d67-fd31-4bb8-9c94-c8906a363a79)


### Question #8:
 We know that the risk classification assigned to a loan represents a customers creditworthiness; higher grades signify lower risk.
 How do loans assigned a grade of A and B differ from all the others?

![8](https://github.com/user-attachments/assets/e6267b14-c216-4481-8ed5-c618f8467152)
![8a](https://github.com/user-attachments/assets/57d1258c-dd1d-4ada-9d8d-dcfb8d2eb513)
![8b](https://github.com/user-attachments/assets/6726ebac-4f54-4791-959c-d504b6e7ddc4)
![8c](https://github.com/user-attachments/assets/0aed79c9-30b6-44db-8a9c-3be95ccc7e7e)
![8e](https://github.com/user-attachments/assets/baedd57d-73e6-41c0-a398-2d8e8b7d8ee4)


### Question #9:
Within risk classification A, which loan purpose has the largest amount of applicants, and which has the least?

![9](https://github.com/user-attachments/assets/9c8c6879-828e-49a3-8ec7-c8fc0f3e3b6e)
![9a](https://github.com/user-attachments/assets/4333c4a9-7613-4252-ac57-ba8dd22c09e0)
![9b](https://github.com/user-attachments/assets/7dd1fd70-8940-4c91-a7a6-99806d315984)


### Question #10: 
Within risk classification A, which loan purpose has the lowest and highest interest rates within this category?

![10](https://github.com/user-attachments/assets/723ab096-6781-4c03-b1a0-dc48340499e4)
![10a](https://github.com/user-attachments/assets/70ef9638-1cfb-4aa4-9b9f-78e55b07245a)


### Question #11: 
Within risk classification A, there are loans with a 36 and 60 month fixed rate. 
What is the distribution of loans within each and their differences by interest rate?

![11](https://github.com/user-attachments/assets/902e57d0-80a5-4939-aa8a-e78f3997a83a)
![11a](https://github.com/user-attachments/assets/49bc6f0d-8778-47c0-8e1b-c6d872126a56)
![11b](https://github.com/user-attachments/assets/bd488662-ddd1-4a08-adf1-7b6a5c27f566)


### Question #12:
Within risk classification A, which home ownership group has the most applications submitted?
Which has the lowest interest rate for a 36 and 60 month term loan?

![12](https://github.com/user-attachments/assets/6abf821d-cda1-4b39-a302-e11e4fb4d859)
![12a](https://github.com/user-attachments/assets/a8a794c4-2f6c-4f8b-913f-60c45355458a)
![12b](https://github.com/user-attachments/assets/ae3325bd-b8c0-4a4b-aa33-305f76b789a5)
![12c](https://github.com/user-attachments/assets/300d14ac-ab4e-446c-9ad7-f099c9f3b401)


### Question #13:
 What states have applicants who pay a mortgage and have the lowest interest rate and DTI Ratio?

 ![13](https://github.com/user-attachments/assets/314bee6e-9d6c-44f2-bf3d-c5ac02ee4544)

 
### Question #14:
 What states have applicants who pay rent and have the lowest interest rate and DTI Ratio?

 ![14](https://github.com/user-attachments/assets/1961e0a6-dcca-4e4d-b84b-29b276b01a06)

 
### Question #15:
What states have applicants who own property and have the lowest interest rate and DTI Ratio?

![15](https://github.com/user-attachments/assets/b292683e-d45a-4d4b-8bf9-73b40a27a612)


## Results from Findings
---

Loans with a risk classification of A have the lowest interest rates within its category, and loan applicants have the lowest DTI ratios overall.

Within risk classification A you have loan type debt consolidation, which is comprised of a majority of the loan applications.

I was able to focus on obtaining customer insights from loans within debt consolidation; those having been fully paid off, and the results obtained are from top applicants in the country who either have a mortgage, pay rent or own property.



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


