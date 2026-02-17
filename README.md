

# Real Estate Data Engineering Pipeline

1️⃣ **Project Overview** 

**📌 Objective**

Designed and implemented a Medallion Architecture pipeline (Bronze → Silver → Gold) to clean and transform raw Airbnb listing data into analytics-ready datasets for business intelligence reporting.


📌 **Business Problem**

Real estate companies collect property listing data including:

   - Price

   - Location

  - Property type

  - Number of bedrooms/bathrooms

  - Listing details

However, raw listing data stored in cloud storage is often inconsistent, incomplete, and not ready for analytics and machine learning.

This project builds an end-to-end data engineering pipeline that:

- Ingests raw listings.csv data from Amazon Web Services S3

- Processes and transforms data using Databricks

- Implements Medallion Architecture (Bronze → Silver → Gold)

- Delivers analytics-ready property insights to Power BI

The final output enables real estate stakeholders to analyze property trends, pricing distribution, and regional performance.

**2️⃣ Architecture Diagram**
![image alt](https://github.com/KatlegoPhoka2/Airbnb-listings/blob/57a241f0f9398515f388354a40a56781ad3ab5aa/architecture%20diagram.png)
**Architecture Benefits**

- Clear data separation

- Improved data quality

- Scalable transformations

- Reliable analytics output
  
**3️⃣Tech Stack Explanation Table**
|Tool|Purpose|Role in Architect|Why It Was Used|
|----|-------|------------------|--------------|
|AWS S3|Raw data storage (Data Lake)|Bronze Layer|Stores immutable raw CSV files, scalable and cost-effective storage, separates storage from compute|
|Databricks|Data transformation & processing|Transformation Engine|Runs distributed data processing jobs, manages Bronze → Silver → Gold pipeline|
|PySpark|Data cleaning & modeling|Silver Layer Cleaning & Gold Aggregation|Cleans messy data, handles large datasets efficiently, pejoins,aggregations, and feature engineering|
|Delta Lake|reliable data storage|Silver & Gold Storage|Provides ACID transactions, prevents corrupted writes, supports schema evolution, enabltime travel|
|SQL|Data querying and aggregation|Gold Layer Analytics|Creates business-ready tables, performs aggregations, enables structured querying for analytics|
|Power BI|Data visualization & reporting|Business Consumption Layer|Builds dashboards, visualizes insights, supports decision-making|
