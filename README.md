

![DWH - Poster](https://github.com/user-attachments/assets/062bfca5-f4c0-4a29-a13c-beaa77f15181)


# Project-Data-WareHouse

This project involves the design and implementation of an Enterprise Data Warehouse (EDW) to integrate data from multiple operational source systems, including `Customer Relationship Management` - (CRM) and `Enterprise Resource Planning` - (ERP) platforms. The goal is to provide a single source of truth for business analytics, reporting, and decision-making.

The solution follows a layered data architecture (`Bronze`, `Silver` & `Gold`) to ensure data quality, scalability, and maintainability.


## 📂 Repository File Structure

    Project-Data-WareHouse
    │
    │
    |
    ├── Datasets/
    |   |     └── CRM
    |   |         ├── customer_info.csv
    |   |         ├── product_info.csv
    |   |         └── sales_details.csv
    |   |
    |   └── ERP
    |       ├── category.csv
    |       ├── cntry.csv
    |       └── customer.csv
    |
    ├── Docs/
    │    ├── Data Architecture.png
    |    ├── Data Catelog.md
    |    ├── Data Flow.png
    |    ├── Data Modeling.png
    │    └── Naming Conventions.md
    |
    |
    ├── Project Scripts
    |    |    |      └── Bronze Layer/
    │    |    |                ├── All Files
    │    |    |                └── Schemas File
    |    |    |  
    │    |    └── Silver Layer/
    |    |                ├── crm_customer_info
    │    |                ├── crm_product_info
    │    |                ├── crm_sales_details    
    │    |                ├── erp_category
    |    |                ├── erp_cntry
    |    |                └── erp_customer
    │    |
    |    └── Gold Layer/
    |             ├── dim_customers   
    │             ├── dim_product
    │             └── fact_sales
    │   
    │
    └── README.md


## 🗒️ Project Tasks  

- **Project Initilization**

- **ETL Pipelines**

- **Data Architecture**


## 🚧 Project Initilization

- **Build Bronze Layer**

- **Build Sliver Layer**

- **Build Gold Layer**


## 🛠️ ETL Pipelines

The ETL process was carefully crafted to move and transform data across the Medallion layers:

**Extract from CSVs → Load to Bronze**

**Transform & Cleanse → Load to Silver**

**Model & Optimize → Load to Gold**


## 💡 Data Architecture

The data structure outlines a **Medallion Architecture** **Bronze**, **Silver** & **Gold** layers.

<img width="851" height="448" alt="Database Layout" src="https://github.com/user-attachments/assets/fd12fdc9-d5b7-4c7b-ae96-37322a0353c1" />


1. **Bronze Layer** - Acts as a landing zone. It stores the data exactly as it appears in the source (like CSV Files).

2. **Silver Layer** - This is the "cleansing" stage where data is validated and made consistent.

3. **Gold Layer** - The final refined stage, optimized for performance and specific business use cases.


## ☍ Links

**[Datasets](Datasets) -** Project CSV files.

