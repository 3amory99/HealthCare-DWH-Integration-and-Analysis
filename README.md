# HealthCare-DWH-Integration-and-Analysis
## Use Case: Data Warehouse Design and ETL Process for Healthcare Data and get insights using SSAS
### Use Case Description and Scenario:

**Goal**:
To design and implement a data warehouse for healthcare data, ensuring data integrity, historical tracking, and effective handling of Slowly Changing Dimensions (SCD). Additionally, to create an OLAP Cube using SQL Server Analysis Services (SSAS) for advanced data analysis.

**Design Data Warehouse**:

The data analyst designs a data warehouse structure to consolidate healthcare data.
The data warehouse includes tables for Billing, Episode, Patient, and Services, each with specific attributes.

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

**Slowly Changing Dimensions (SCD)**:

* Slowly Changing Dimensions (SCD) are applied to certain dimension tables, such as the Patient and Services dimensions.
* The purpose of SCD is to manage historical changes in dimension attributes over time.
* Specifically, Type 2 SCD is implemented to track changes, ensuring that historical versions of dimension data are preserved.
* This is crucial for historical reporting and analysis, allowing for retrospective examination of healthcare data.

**Postconditions**:

The healthcare data is successfully loaded into the data warehouse.
Data integrity is maintained between fact and dimension tables.
Historical changes are tracked using the Date Dimension.
Slowly Changing Dimensions (Type 2) effectively manage historical changes in dimension data.
An OLAP Cube is created using SSAS, enabling advanced multidimensional healthcare data analysis.

**SSAS OLAP Analysis Cube**:
SQL Server Analysis Services (SSAS) is used to create an OLAP Cube.
An all-star schema is implemented within the OLAP Cube, connecting the fact table (Billing) to dimension tables (Episode, Patient, and Services).
The OLAP Cube provides a multidimensional view of healthcare data, enabling advanced analytics and data exploration.

**Datawarehouse Star Schema**:

![Datawarehouse Star Schema](https://github.com/3amory99/HealthCare-DWH-Integration-and-Analysis/blob/master/images/star%20schema.PNG)

**SSIS Package**:

![SSIS Package](https://github.com/3amory99/HealthCare-DWH-Integration-and-Analysis/blob/master/images/SSIS%20Package.PNG)

**Patient Dimension Data Flow**:

![Patient Dimension Data Flow](https://github.com/3amory99/HealthCare-DWH-Integration-and-Analysis/blob/master/images/DFT_DimPatients.PNG)

**SSAS OLAP Cube**

![SSAS OLAP Cube](https://github.com/3amory99/HealthCare-DWH-Integration-and-Analysis/blob/master/images/Analysis%20cube.PNG)


