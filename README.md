# **Sales Management Project using PowerBI and SQL**


![Overview](Images/Overview.png)


## **Business Request and User Stories**

The business request for this data analyst project was an executive sales report for sales managers. Based on the request that was made from the business, we defined the following user stories to fulfill delivery and to ensure that acceptance criteria were maintained throughout the project.
| **No.** | **As a (role)** | **I want (request / demand)** | **So that I (user value)** | **Acceptance Criteria** |
| :--- | :----------- | :-------- | :------- | :------------------------- |
| 1   | Sales Manager | A dashboard overview of sales in year 2020 and 2021 | Can follow better which customers and products sells the best | A Power BI dashboard which let us see top 10 products and customers after applying different filters available on dashboard |
| 2   | Sales Manager | A dashboard overview of sales and budget | Can follow sales over time against budget | A Power BI dashboard with graph comparing against budget |
| 3   | Sales Representative | A detailed overview of Sales per Customer | Can follow up my customers that buys the most and who we can sell more to | A Power BI dashboard which allows me to filter data for each customer |
| 4   | Sales Representative | A detailed overview of Sales per Product | Can follow up my Products that sells the most | A Power BI dashboard which allows me to filter data for each Product |

## **Data Cleansing & Transformation (SQL)**

- To create the necessary data model for doing analysis and fulfilling the business needs defined in the user stories the following tables were extracted using SQL.
- One data source [_FACT_SentSalesBudget_](Data_for_Power_BI/FACT_SentSalesBudget.xlsx) were provided in Excel format and were connected in the data model in a later step of the process.
- Below are the SQL statements for cleansing and transforming necessary data.

  1. [_DIM_Calendar.sql_](SQL_Queries/DIM_Calendar.sql)
  2. [_DIM_Customers.sql_](SQL_Queries/DIM_Customers.sql)
  3. [_DIM_Product.sql_](SQL_Queries/DIM_Product.sql)
  4. [_FACT_InternetSales.sql_](SQL_Queries/FACT_InternetSales.sql)


![SQL_Queries_Collage](Images/SQL_Queries_Collage.png)


## **Data Model**

Below is a screenshot of the data model after cleansed, prepared tables were read into Power BI and after creating required measures.

This data model also shows how [_FACT_InternetSales_](Data_for_Power_BI/FACT_InternetSales.csv) and [_FACT_Budget_](Data_for_Power_BI/FACT_SentSalesBudget.xlsx) has been connected to other necessary DIM tables.


![Data Model](Images/Data_Modelling_Screenshot.png)


## **Sales Management Dashboard**

The finished sales management dashboard with first page which works as both dashboard and as overview of sales and budget, with two other pages focused on combining tables for necessary details and visualizations to show sales over time per customers and per products respectively.

Final report can be downloaded using the link: [Sales_Report_Final.pbix](Sales_Report_Final.pbix). It needs Power BI Desktop installed in PC to open that file.

Below are the screenshots of the Sales_Report_Final.pbix report:


![Sales_Overview_Screenshot.png](Images/Sales_Overview_Screenshot.png)


![Customer_Details_Screenshot.png](Images/Customer_Details_Screenshot.png)


![Product_Details_Screenshot.png](Images/Product_Details_Screenshot.png)


### _**Thank you for your valuable time**_
