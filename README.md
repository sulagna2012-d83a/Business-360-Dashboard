📊 AtliQ Hardware (Power BI Data Analytics Project)
Project Overview

AtliQ Hardware is a fast-growing global company selling computers and accessories. To move away from intuition- and Excel-based decisions—which previously led to losses, especially in the American market—the company adopted Power BI–driven analytics.
This project delivers an end-to-end Power BI dashboard providing insights across Finance, Sales, Marketing, Supply Chain, and Executive management, enabling data-driven decision-making and competitive advantage.

🛠 Tech Stack Used

•	SQL

•	Power BI Desktop

•	Microsoft Excel

•	DAX Language

•	DAX Studio (for performance optimization)

•	Project Charter Document

🏢 Company Background

AtliQ Hardware operates worldwide and sells computer products through three main sales channels:

•	Retailers

•	Direct Sales

•	Distributors

The company serves customers through:

•	Brick & Mortar stores (offline)

•	E-commerce platforms (Amazon, Flipkart)

Due to recent losses and growing competition, management decided to invest in analytics to improve future business decisions.

🎯 Project Kick-Off & Business Requirements:

Before starting dashboard development, a kick-off meeting was conducted to clearly understand business goals and expectations.
Key Questions Asked:

1	What is the main objective of building this Power BI dashboard?

2 How will the success of this project be measured?

3	What is the project deadline?

4	Do stakeholders expect a preview before final release?

4	What insights do stakeholders expect from this dashboard?

5	What are their concerns or risks regarding this project?

6	Who will use the dashboard and for what purpose?

7	What problems might occur during development?

8	What data and resources are required?

9	Are there any design or visualization preferences?

📂 Dataset Understanding

Understanding the data was a crucial step before starting analysis.

1.Dimension Tables

    Contain static information such as customers, products and markets.
    
    
    -> gdb041


•	dim_customer

     -27 Distinct markets (India, USA, Spain, etc.)
     
     -75 Distinct customers
     
     -2 platforms: 
         > Brick & Mortar
         > E-commerce

     -3 channels:
         > Retailer
         > Direct
         > Distributor

•	dim_market

     o	27 markets
     
     o	7 sub-zones
     
     o	4 regions: 
          > APAC
          > EU
          > LATAM
          >  NAN
     
•	dim_product

    o	Divisions
    
    o	P & A 
           > Peripherals
           >  Accessories)
    
    o	PC 
           > Notebook
           > Desktop)
    
    o	N & S 
            > Networking 
            > Storage
    
    o	14 product categories 
              > Keyboard
              > Internal HDD, etc.)
    
    o	Multiple variants per product
    
2.Fact Tables

    Contain transactional and quantitative data.
    
•	fact_forecast_monthly

    o	Forecasted customer demand
    
    o	Helps in inventory planning and cost reduction
    
    o	Dates stored as start of the month
    
    o	Final column contains forecast quantity
    
•	fact_sales_monthly

    o	Similar structure to forecast table
    
    o	Final column contains actual sold quantity
    
    
    -> gdb056

•	freight_cost – Transportation cost by market and fiscal year

•	gross_price – Product gross prices

•	manufacturing_cost – Manufacturing cost by product and year

•	pre_invoice_deductions – Pre-invoice discount percentages by customer

•	post_invoice_deductions – Post-invoice discounts and deductions

🔌 Data Import

The data source for this project was MySQL.

All tables were imported into Power BI using database credentials.


🧩 Data Modeling

•	Data modeling was designed carefully as it directly affects report performance.

•	Followed best practices for analytics modeling.

•	Used Snowflake schema for better scalability and performance.

![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/4b397b6fc59c63f861d3d3a00007f1b502d5b405/Data%20Model.jpg)


•	All measures and visuals were built on top of this optimized model.

🎨 Dashboard Design

Based on stakeholder mockups and requirements, multiple views were created with interactive visuals and DAX measures.

Dashboard Structure:


- **Home View**: Serves as the main navigation hub for the entire report
  
- **Info View**: Provides project and dashboard-related information  

•	Finance View
    ![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/bf96d306d116d4755ffc03adb4de6e34bec3c498/Finance%20View%20.jpg)

    Unveil an Profit and Loss Statements for financial performance across Markets Products,Customers and list down the Top and Bottom Products and Customer Net Sales

•	Sales View
   ![iage_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/e33d44848a970e694c4dd374b776e641152fa7a3/Sales%20view.jpg)

     Decode customer and product performances influenced by Key metrics such as Net Sales and Gross Margin Percentage ,make an performance matrix b/w NS and Np % for market, customer as values ,then explore the Break down for Needful P & L values of Sales View such as Net Sales , COGS , Gross Marigin.

•	Marketing View
  ![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/2207c2ffa665eaeab081af489251bcbda586db3d/Marketing%20View.jpg)

  Discover Region and market performances influenced by Key metrics such as NS,NS%,GM,GM% ,make an performance matrix b/w NS and GM % for segment, category as Values ,then explore the Break down of Needful P & L values for Marketing View such as Gross Marigin ,Operational Expenses



•	Supply Chain View
   ![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/fe5f0b78c0e2efde4907e0b8912efffa4f9f986d/Supply%20Chain%20View.jpg)

   Track the Customer and Product Key Metrics such as Forecast Accuracy,FA%,Net Error,NE%,ABS Error ,Also plot an Trendline over the Selected period of Net Error and Forecast Accuracy

•	Executive View
  ![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/0d3a2b6d12f8b261b4bbe5545bc7117cb6cc2efc/Executive%20View%20N.jpg)

  Evaluating departmental performance at a glance by plotting Yearly Trends of KPI’s (GM %,NP%, Market share%), Market Share Trends etc.., which enables business leaders to bridge gap between strategy and results by closely monitoring and managing the execution of initiatives.

 Also i have added a Support page for further assistance.


Each view provides focused insights for different business teams.


✅ Project Outcome

•	Enabled stakeholders to track performance across departments

•	Improved decision-making using real business data

•	Reduced dependency on manual Excel analysis

•	Built a scalable analytics foundation for future growth

