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


•	All measures and visuals were built on top of this optimized model.

🎨 Dashboard Design

Based on stakeholder mockups and requirements, multiple views were created with interactive visuals and DAX measures.

Dashboard Views:

•	Home View – Navigation hub for all reports

•	Info

•	Finance View

•	Sales View

•	Marketing View

•	Supply Chain View

•	Executive View
  ![image_alt](https://github.com/sulagna2012-d83a/Business-360-Dashboard/blob/4d166fa6f06b032a96104e1a20cce9d61232e6cf/Executive%20View.jpg)

•	Products

•	Support

•	Overall Performance Report

Each view provides focused insights for different business teams.


✅ Project Outcome

•	Enabled stakeholders to track performance across departments

•	Improved decision-making using real business data

•	Reduced dependency on manual Excel analysis

•	Built a scalable analytics foundation for future growth

