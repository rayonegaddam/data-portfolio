## Sales Analysis Data Pipeline

Objective:
This project demonstrates an end-to-end data workflow for analyzing retail sales data. It covers reading raw data, cleaning and transforming it using Python, storing it in a MySQL database, and visualizing insights through Power BI.

⚙️ Tech Stack: Python, MySQL, PowerBI

✅ Dataset Overview
Fields:

OrderID, Order Date

Country, State, City, Region

Segment, Ship Mode, Category, Sub-Category

Discount, Sales, Profit

Volume: ~8,037 rows

📌 Workflow

1️⃣ Data Reading & Exploration
Loaded data using Pandas (read_csv).

Explored structure with .shape, .info(), .describe(), .unique().

2️⃣ Data Cleaning
Dropped nulls and exact duplicates.

Checked for logical errors:

Negative sales or profit

Discounts > 100%

Verified data types (datetime, float, category).

Normalized text fields for consistency.

3️⃣ Data Transformation
Created new date features: year, month.

Verified uniqueness of order_id as needed.

Saved the final cleaned DataFrame.

4️⃣ Data Modelling
Used SQLAlchemy and PyMySQL to export the clean DataFrame to a MySQL database table (cleaned_orders).

Defined a clear schema with correct column types for reporting.

5️⃣ Reporting
Connected Power BI Desktop to the MySQL database.

Built interactive dashboards
