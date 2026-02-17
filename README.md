

# Real Estate Data Engineering Pipeline

1️⃣ **Project Overview** 

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
