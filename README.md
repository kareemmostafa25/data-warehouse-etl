Kareem Mostafa Data Warehouse ETL

This is a simple ETL project for my Data Warehouse course.
The main goal is to practice the ETL steps (Extract, Transform, Load) using SQL Server.

 Layers

Bronze Layer → Raw data tables (imported as they are).

Silver Layer → Cleaned and transformed data (fixed datatypes, added record_insert_dt, etc.).

Gold Layer → Business reports (top products, top customers, low sales).

 Tables Used

CRM_CUST_INFO → Customer information.

CRM_PRD_INFO → Product information.

CRM_SALES_DETAILS → Sales orders.

ERP_CUST_AZ12 → Extra customer data.

ERP_LOC_A101 → Location data.

ERP_PX_CAT_G1V2 → Product categories.

 ETL Idea

Extract: Load raw data into Bronze schema.

Transform:

Convert data types.

Add audit columns (record_insert_dt).

Join datasets (e.g., sales + products + customers).

Load: Insert the cleaned/transformed data into Silver schema.

Then aggregate reports in the Gold schema (top selling products, top customers, low sales).

 Tools

SQL Server
