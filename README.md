🏠 Real Estate BI Analytics — Power BI Project
📌 Project Overview

This project focuses on building interactive Power BI dashboards to analyze the Moroccan real estate market using data collected from Avito.ma.

The Data Warehouse is organized into two schemas:

bi_schema → Used for Business Intelligence and reporting
ml_schema → Reserved for Machine Learning (not used in this project)

This project uses only the BI layer to create dynamic and analytical dashboards.

🎯 Objectives
Connect Power BI to the Data Warehouse
Import tables from bi_schema
Prepare data using Power Query
Create KPIs and measures with DAX
Build interactive dashboards for real estate analysis

📊 Dashboards
Dashboard 1 — Global Market Overview
Total listings
Average price
Listings by city
Market evolution

Dashboard 2 — Price Analysis
Price distribution
Average price per m²
Segment comparison

Dashboard 3 — Geographic Analysis
Listings by city
Geographic price visualization
Most expensive areas

Dashboard 4 — Trend Analysis
Price evolution
Listings evolution
Seasonal trends

🎛️ Interactive Filters
City
Property type
Price range
Surface
Period\

🛠️ Technologies Used
Power BI
Power Query
DAX
PostgreSQL
SQL
Python

🏗️ Data Warehouse Structure
bi_schema
│
├── fact_annonces
├── dim_ville
├── dim_date
├── dim_type_bien
└── dim_surface

🚀 Workflow
Data Collection
      ↓
ETL Pipeline
      ↓
Data Warehouse
      ↓
Power BI
      ↓
Dashboards & KPIs
