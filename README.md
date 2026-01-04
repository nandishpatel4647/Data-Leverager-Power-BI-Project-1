📊 Data Leverager – Power BI ETL (Power Query) Project
📌 Project Overview

Data Leverager is an internal ETL-focused Power BI project designed to simulate a real-world data engineering workflow.
The project focuses entirely on data extraction, cleaning, transformation, integration, and quality validation using Power BI Power Query, with no use of DAX or visualizations.

This project demonstrates hands-on expertise in building a scalable and refreshable ETL pipeline using industry best practices.

🎯 Objective

To extract data from multiple sources, perform structured data transformations, and prepare high-quality, analysis-ready datasets using Power BI’s Power Query Editor.

🧩 Data Sources

Folder-based Excel Sales Data

Sales_Jan.xlsx

Sales_Feb.xlsx

Sales_Mar.xlsx

Sales_Apr.xlsx (refresh simulation)

Employee Master Data

Employees.xlsx

Web Data

HTML table sourced from Wikipedia (country-wise data)

🔄 ETL & Transformations Performed
1. Data Extraction

Loaded multiple Excel files dynamically using Folder connector

Combined monthly sales files using Append Queries

Loaded employee data from Excel

Extracted structured data from a web HTML source

2. Data Cleaning & Preparation

Removed blank rows and columns

Promoted first row as headers

Renamed columns for clarity

Changed data types using Change Type with Locale

Removed duplicates and filtered null values

3. Text Transformations

Standardized customer names using:

UPPER

TRIM

CLEAN

Replaced inconsistent text values

Split address fields using delimiters

4. Numeric Transformations

Rounded revenue and cost values to 2 decimal places

Created calculated Profit column:

Profit = Revenue - Cost

5. Date & Time Transformations

Extracted:

Day

Month

Year

Quarter

Created Fiscal Month column

Calculated employee Age from Birthdate

6. Conditional Columns & Indexing

Created Sales Category column:

High (≥ 10,000)

Medium (5,000–9,999)

Low (< 5,000)

Added Index columns:

0-based

1-based

7. Pivoting & Unpivoting

Pivoted monthly data for transformation demonstration

Unpivoted data back into normalized structure

8. Merging & Appending

Merged Sales data with Employee data using EmployeeID

Appended all monthly sales data into a single fact table

9. Grouping & Aggregation

Grouped data by Region to compute:

Total Sales

Average Order Value

Transaction Count

10. Data Profiling & Quality Checks

Enabled:

Column Quality

Column Distribution

Column Profile

Identified missing values, errors, and unique values

11. Parameters & Source Management

Created a FolderPath parameter for dynamic file loading

Configured data source credentials

Ensured portability and refresh stability

12. Refresh Simulation

Added a new monthly file (Sales_Apr.xlsx)

Verified automatic data ingestion on refresh

Confirmed all transformation steps remained intact

🛠 Tools & Technologies

Power BI Desktop

Power Query Editor

Excel (Data Source)

Web HTML Data Source

🚫 Out of Scope

No DAX measures

No Power BI visualizations

No report or dashboard layer

📦 Deliverables

Power BI .pbix file with all Power Query transformations

Structured ETL pipeline with dynamic refresh capability

Clean, normalized, analysis-ready datasets

✅ Key Learnings

Folder-based ETL automation

Parameter-driven data pipelines

Data quality validation techniques

Real-world Power BI ETL best practices

👤 Author

Nandish Patel
B.Tech in AI & ML (2028)
Diploma in Information Technology
ETL | Power BI | Data Analytics

📄 License

This project is intended for educational and internal evaluation purposes only.
