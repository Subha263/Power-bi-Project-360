# Power-bi-Project-360
Project Overview
---
AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

I worked on this project by following the Codebasics PowerBi Course,and the live dashboard line is [here](https://app.powerbi.com/view?r=eyJrIjoiOWExMDVmNmUtMWM1Zi00ODY1LThhYmUtY2RhMjk5NjJlNGZkIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

Tech stacks
---
* SQL

* PowerBi Desktop
  
* Excel
  
* DAX language

* DAX studio (for optimizing the report)
  
* Project charter file

  PowerBI techniques Learned
  ---
* What are all the questions should be asked before staring the project

* Creating calculated columns

* creating measure using DAX language

* Data modeling

* Using Bookmarks to switch between two visuals

* Page navigation with buttons

* Using divide function to prevent zero division errors

* creating date table using m language

* Dynamic titles based on the applied filters

* Using KPI indicators

* Conditional formatting the values in visuals using icons or background color

* Data validation techniques

* PowerBi services

* Publishing reports to PowerBi services

* Setting up personal gateway to set up the auto refresh of data

* PowerBi App creation

* Collaboration, workspace, access permissions in PowerBi services

* And more 😅

Business related terms
---
* Gross price

* Pre-invoice deductions

* Post-Invoice deductions

* Net Invoice sale

* Gross Margin

* Net sales

* Net profit

* COGC - cost of goods sold

* YTD - Year to Date

* YTG - Year to Go

* Direct

* Retailer

* Distributors

* Consumer

Company’s back ground
---
AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

* Retailers

* Direct

* Distributors

Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry.
Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

Questions to ask before starting with dashboard
---
* What is the objective of building this PowerBi dashboard?
* In what terms the success of this project will be measured?
* What will be time dead-line of the project?
* Do the stakeholders expecting pre-view before the actual release?
* What are all the hopes stakeholders have out of this project?
* what are all fears the stakeholder have in terms of building this dashboard?
* Who are all will be using this dashboard and for what purpose?
* what are all expectation the stakeholders have, by the completion of this project?
* What can go wrong while building this project?
* what are all the resources/ data needed to build this dashboard?
* Is there any inputs from stakeholders in terms of design and views of the dashboard?
* After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

  Dataset Understanding.
  ---
Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.
Dimension table : It will have the static data like details of customer and products
Fact table : It will have the data about the transactions

* gdb041:
  
 **dim_customer table contains following information**
* 27 distinct markets (ex India, USA, spain)
* 75 distinct customers thorough out the market
* 2 types of platforms
  Brick & Motors - Physical/offline store and 
  E-commerce - Online Store (Amazon, flipkart)
* Three channels (Retailer,Direct,Distributors)
* 
**dim_market table contains following information**

* 27 distinct markets (ex India, USA, spain)
* 7 sub-zones
* 4 regions(APAC,EU,Nan,LATAM)
  
**dim_product table contains following information**

* Divisions
* P & A(Peripherals,Accessories)
* PC(Notebook,Desktop)
* N & S(Networking,Storage)
* There are 14 different categories, Like Internal HDD, keyboard
* There are different variants available for the same product
  
**fact_forecast_monthly table contains following information**

* This table is used to forecast the customer’s need in advance, which can help in-----
*  higher customer satisfaction
* Reduced cost in warehouses for storage purpose
* The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
* All the date of the month will be replaced by the start date of the month
* It will have all the column names and in the end it will have the forecast quantity need of the customer
  
**fact_sales_monthly table** 
* This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
  
* gdb056
  
**freight_cost table**
* This table has details of travel cost and other cost for each market with fiscal year
  
**gross_price table**
* Has the details of gross prices with product code
  
**manufacturing_cost table**
* Has the details of manufacturing cost with product code with year
  
**Pre_invoice_dedutions table**
* Has the details of pre invoice deductions percentage for each cutomer with year
  
**Post_invoice_deductions table**
* Post invoice deductions and other deductions details
  
  Importing data into PowerBi
  ---
As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing 
the Database access credential

Data Model
---
* Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
* Poor data modeling affects the over all performance of the report.
* In this project, we have followed Snowfall data modeling method.
<img width="720" alt="Project_Screenshot2_updated" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/ca6b7f46-9800-488c-a13b-f49840c27334">

Dashboard designing
---
Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

Home view
---
In Home view, all the views button will be available. User will land on specific view page by clicking the button

* Info
* Finance View
* Sales View
* Marketing View
* Supply chain View
* Executive View
* Products
* Support
  <img width="720" alt="home-pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/9b57d74d-793b-4285-8b49-153fb2cf452c">

Finance View
---
<img width="720" alt="finance -pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/196f8a35-aa2e-4031-8452-6bf744f68a6a">

Sales View
---
<img width="720" alt="sales-pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/9fd25345-03bd-4767-bcb9-ea0abf7131c8">

Marketing View
---
<img width="804" alt="marketing-pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/50ae27f1-477a-4b7d-b8fa-eb227864e488">


Supply chain View
---
<img width="805" alt="supply-pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/8d9601aa-64f9-4cb7-a80b-4680af021b73">

Executive View
---
<img width="689" alt="executive-pic" src="https://github.com/Subha263/Power-bi-Project-360/assets/146601418/f04e8dd8-80ce-4386-9d22-c9aa1301309b">

you can find the full report file [here](https://app.powerbi.com/view?r=eyJrIjoiOWExMDVmNmUtMWM1Zi00ODY1LThhYmUtY2RhMjk5NjJlNGZkIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9
)

Project Outcome
---
By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
  





