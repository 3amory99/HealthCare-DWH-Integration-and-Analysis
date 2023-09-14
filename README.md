# HealthCare-DWH-Integration-and-Analysis
## Use Case: Data Warehouse Design and ETL Process for Healthcare Data and get insights using SSAS
### Use Case Description and Scenario:

**Design Data Warehouse**:

The data analyst designs a data warehouse structure to consolidate healthcare data.
The data warehouse includes tables for Billing, Episode, Patient, and Services, each with specific attributes.

**Type of Data Warehouse**:

The chosen type of data warehouse is a "Kimball-style" data warehouse.
This design choice is made because it provides a dimensional model that is well-suited for healthcare data analytics, offering flexibility and ease of querying.

**Maintain Data Integrity**:

The data analyst defines SQL-based methods to maintain data integrity between fact (Billing and Episode) and dimension (Patient and Services) tables.
Integrity checks and constraints are implemented to ensure accurate and consistent data.

**Date Dimension Addition**:

A Date Dimension table is added to the system to track historical changes in healthcare data.
This enables time-based analysis and historical reporting.

**SSIS ETL Project**:

An SSIS (SQL Server Integration Services) project is designed to automate the Extraction, Transformation, and Loading (ETL) process.
The ETL process extracts data from Excel files (Billing, Episode, Patient, Services) and populates the data warehouse tables.
Data transformation steps include segmentation, tokenization, and other NLP preprocessing techniques as needed.
Historical data is tracked using the Date Dimension.

**Database Star Schema**
![Database Star Schema](https://github.com/3amory99/HealthCare-DWH-Integration-and-Analysis/blob/master/images/star%20schema.PNG)

