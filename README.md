# Business Insights 360

Live Dashboard [Link](https://www.novypro.com/project/business-insights-360-power-bi-14)

## Project Overview

The project was done on a well-crafted dataset of a hypothetical company called Atliq Hardware. The goal of the project was to build an automated Power BI dashboard for the finance, sales, marketing, and supply chain teams at Atliq, to help them analyze the data effectively for better decision-making.

AtliQ Hardwares is a consumer electronics company expanding rapidly but is not able to compete with other companies using data as most of their report still exists in Excel. My goal is to implement an advanced analytics solution using Power BI that will enable the company to get insights and make informed decisions.


I worked on this project by following the Codebasics PowerBi Bootcamp, Link to the course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

[Live Report Link](https://www.novypro.com/project/business-insights-360-power-bi-14)

## Tech stacks

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI techniques used

- Stakeholder Feedback Implementation
- Dashboard designing principles
- Power Query (Basic and Advanced Operations) 
- Basic and complex DAX formulas
- Data modeling involving 10+ tables
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Creating date table using m language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- Deploying in Power BI service
- Setting up personal gateway to set up the auto refresh of data
- PowerBI App creation
- Collaboration, workspace, access permissions in PowerBi services
- Sales, Marketing, Finance & Supply Chain metrics
- Basic queries in MySQL and loading data from MySQL database to power BI.
-  Data Validation using Excel.


## Business related terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sale
- Gross Margin
- Net sales
- Net profit
- COGC - cost of goods sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

## Company’s back ground

AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry. 

Project kick off session, where you should get clear of for what and why this project and all other questions you have with regards to the project

### Questions to ask before starting with dashboard

- What is the objective of building this PowerBi dashboard?
- In what terms the success of this project will be measured?
- What will be time dead-line of the project?
- Do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- What are all fears the stakeholder have in terms of building this dashboard?
- Who are all will be using this dashboard and for what purpose?
- What are all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Is there any inputs from stakeholders in terms of design and views of the dashboard?

After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

### Dataset **Understanding.**

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
        - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details

## Importing data into PowerBi

- As the database is MySQL in this project, we need to import the datasets from Mysql database to PowerBi by providing the Database access credential

## Data Model

- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the over all performance of the report.
- Following Good practices of data modeling is must. Refer this page to get to know the good practices [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- In this project, we have followed Snowfall data modeling method.

<img src="https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Data_model.png" class="center">

### Dashboard designing

Based on the mock ups received as requirement, the team will start designing the visuals and create measure as and when required

## Home view

In Home view, all the views button will be available. User will land on specific view page by clicking the button 

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Products
- Support

## Overall Report

![Overall Report.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Overall.gif)

## Info Page

![Info.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Info.gif)

## Finance View

![Finace.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Finace.gif)
## Sales View

![Sales.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Sales.gif)

## Marketing View

![Marketing.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Marketing.gif)

## Supply chain View

![Supply chain.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/supply%20chain.gif)

## Executive View

![Executive.gif](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Executive.gif)

## Products

![Products](https://github.com/Gaboytes/Business_Insights_360/blob/main/Resources/Products%20View.gif)

you can find the full report file here : [Report](https://github.com/Gaboytes/Business_Insights_360/tree/main/Report)


## Project Outcome

By using this report, decisions can be taken based on the data. Further it will help in answering n number of why questions based on the situations.
