```markdown
# Data Warehouse and Analytics Project

A complete end to end data warehousing and analytics project built using SQL Server.  
This repository demonstrates modern data engineering practices, analytical data modeling, and business focused SQL analytics.

This project is designed as a strong portfolio artifact for Data Analyst, Analytics Engineer, and BI focused roles.

---

## Project Objective

Build a modern data warehouse that consolidates ERP and CRM sales data into a single analytical model.

Enable decision making through clean, reliable, and analytics ready data.

---

## Data Architecture

The project follows the Medallion Architecture pattern with three layers.

Bronze Layer  
Stores raw data ingested directly from source systems without transformation.

Silver Layer  
Handles data cleansing, validation, standardization, and normalization.

Gold Layer  
Contains business ready data modeled using a star schema for reporting and analytics.

Architecture diagram is available in docs/data_architecture.png.

---

## Data Sources

ERP System  
Contains transactional sales and product level data.

CRM System  
Contains customer profiles and engagement attributes.

Both sources are provided as CSV files and loaded into SQL Server.

---

## ETL Pipeline

Extraction  
Raw CSV files are loaded into Bronze tables using SQL based ingestion scripts.

Transformation  
Silver layer applies data quality rules including:
- Null handling
- Deduplication
- Case standardization
- Invalid date correction
- Negative value fixes

Loading  
Gold layer tables are created using dimensional modeling techniques.

All ETL logic is implemented using SQL.

---

## Data Modeling

The Gold layer follows a star schema design.

Fact Table  
FactSales  
Stores transactional metrics such as revenue, quantity, and order count.

Dimension Tables  
DimCustomer  
DimProduct  
DimDate  
DimRegion or Channel depending on availability

This model supports fast analytical queries and simplified reporting.

Data model diagram is available in docs/data_models.drawio.

---

## Analytics and Reporting

SQL based analytics answer core business questions.

Customer Analytics  
Customer lifetime value  
Repeat purchase behavior  
Top customers by revenue  
Customer segmentation trends  

Product Analytics  
Top performing products  
Low performing products  
Category level performance  
Price and volume analysis  

Sales Analytics  
Month over month growth  
Year to date trends  
Seasonality patterns  
Regional performance  

All analytics queries are reusable and documented.

---

## Repository Structure

```

data-warehouse-project/
│
├── datasets/                # Raw ERP and CRM CSV files
│
├── docs/                    # Architecture, models, and documentation
│   ├── etl.drawio
│   ├── data_architecture.drawio
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── data_catalog.md
│   ├── naming-conventions.md
│
├── scripts/
│   ├── bronze/              # Raw ingestion scripts
│   ├── silver/              # Data cleansing and transformation scripts
│   ├── gold/                # Star schema and analytics tables
│
├── tests/                   # Data quality and validation scripts
│
├── README.md
├── LICENSE
└── requirements.txt

```

---

## Tools and Technologies

SQL Server Express  
SQL Server Management Studio  
Draw.io  
Git and GitHub  

---

## Skills Demonstrated

SQL development  
Data warehousing design  
ETL pipeline implementation  
Star schema data modeling  
Business driven analytics  
Data quality management  
Technical documentation  

---

## How to Run the Project

Install SQL Server Express  
Install SQL Server Management Studio  

Clone this repository  
Load CSV files from the datasets folder  

Execute scripts in this order:
1. Bronze layer
2. Silver layer
3. Gold layer

Run analytics queries on Gold layer tables.

---

## Use Cases

Portfolio project for data analytics and BI roles  
Interview discussion project covering architecture and analytics  
Reference implementation for SQL based data warehousing  

---

## About Me

Saswata Ghosh  
Product Designer, UI UX Designer, Frontend Developer, Data Analytics Enthusiast

I build systems that combine design clarity, technical structure, and analytics driven insight.  
My focus is on data informed products and scalable analytical workflows.

---

## Connect

Portfolio  
https://saswataghosh.vercel.app  

LinkedIn  
https://linkedin.com/in/saswata-ghosh06  

GitHub  
https://github.com/Saswataghosh06  

Email  
saswataghosh2022@gmail.com  

---

## License

This project is licensed under the MIT License.  
Free to use, modify, and distribute with attribution.
```

