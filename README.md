Introduction

This project is a dashboard for Ghabbour Company built using Power BI. The goal is to analyze sales performance and track KPIs interactively to help in decision-making.

Data Preparation (Power Query)

At the beginning, I worked on cleaning the data using Power Query:

Removed duplicates
Handled missing values
Performed data type transformation (dates – numbers)
Created calculated columns such as (Year / Quarter)
Converted all primary keys and foreign keys to text, or more precisely changed their formatting, to help me in Data Modeling
Data Modeling

I removed everything that was automatically created by Power BI and started building the relationships myself so they would be easier and faster in Power BI and make the analysis smarter and without errors.

I really needed to create a relationship between two fact tables, but I didn’t do it because it is not the best practice in analysis
I could have created a bridge table, but instead I worked using DAX through TREATAS
DAX Calculations

I used DAX to create basic measures such as:

Total Sales
Total Transactions
Total Quantity
Sales Percentage

I also used functions such as:

CALCULATE
SUMX
TOPN
ALL
TREATAS
Dashboard

The dashboard is divided into several sections:

Total Transactions (5K)
Total Quantity (24.4K)
Total Invoices (44bn)
Total Revenue

The goal is to provide a high-level view.

Sales comparison by year (2024 vs 2025)
Quarterly trend analysis

This helps us understand trends and seasonality.

Analysis of number of invoices per Sales Rep
Completed transactions
Cancelled transactions

From this, we can evaluate each employee’s performance and identify the highest and lowest performers.

Customer distribution by gender (Male vs Female)

This helps in understanding customer behavior.

Here, I had to use DAX to get the correct numbers based on completed transactions for each seller, and not rely on the numbers موجودة in another table because many transactions were cancelled.

After that, I analyze warehouse movement and the number of units available in each warehouse

This helps us know which products and models are most requested so we can keep supplying the warehouses with them, and which ones have low demand so we can start making offers on them or increase their marketing.






<img width="1449" height="797" alt="غبور2" src="https://github.com/user-attachments/assets/252c564b-6a79-49a9-b0d5-3b0ce56eb073" />
<img width="1403" height="790" alt="غبور3" src="https://github.com/user-attachments/assets/7cf34f1d-a285-47e1-ae5c-7e428424b484" />
<img width="1387" height="794" alt="غبور4" src="https://github.com/user-attachments/assets/d9fe36ec-3fdd-447f-884b-7a845f638229" />
<img width="1391" height="794" alt="غبور5" src="https://github.com/user-attachments/assets/2dc23f60-ae36-4789-9f21-9b325e39093e" />
<img width="1379" height="796" alt="غبور6" src="https://github.com/user-attachments/assets/55fc88ef-4a04-45bc-8290-7e152e198891" />
<img width="1459" height="171" alt="غبور7" src="https://github.com/user-attachments/assets/3293831f-fcc6-4c64-b704-027c65c43427" />
<img width="1357" height="151" alt="غبور8" src="https://github.com/user-attachments/assets/df9daf89-5cce-4b50-bef8-94d57e1bacd1" />












Then I move to analyzing the dealers we work with in terms of their number, locations, who deals the most with the company, whose transactions are completed, who cancels, and their evaluation
