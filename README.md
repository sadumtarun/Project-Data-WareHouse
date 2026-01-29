# Project-Data-WareHouse

This project involves the design and implementation of an Enterprise Data Warehouse (EDW) to integrate data from multiple operational source systems, including Customer Relationship Management (CRM) and Enterprise Resource Planning (ERP) platforms. The goal is to provide a single source of truth for business analytics, reporting, and decision-making.

The solution follows a layered data architecture (Bronze, Silver, Gold) to ensure data quality, scalability, and maintainability.


## 📂 Repository File Structure

    sql-data-warehouse-project/
    │
    ├── README.md
    │
    ├── Docs/
    │   ├── architecture.png
    │   └── data_model.png
    │
    ├── Bronze Layer/
    │   ├── All Files
    │   ├── Schemas File
    │   ├── 
    │   ├── 
    │   └── 
    │
    ├── Silver Layer/
    │   ├── crm_customer_info
    │   ├── crm_product_info
    │   ├── crm_sales_details
    |   ├── erp_category
    |   ├── erp_cntry
    │   └── erp_customer
    │
    ├── Gold Layer/
    │   ├── dim_customers
    │   ├── dim_product
    │   └── fact_sales
    │
    ├── Validation/
    │   ├── data_quality_checks
    │


## 🗒️ Project Tasks  

- **Project Initilization**

- **ETL Pipelines**

- **Overarching Principles**

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

## ✒️ Overarching Principles

### Rules

- **Naming conventions** - Use snake_case, separating words with underscores (_) and lowercase letters.
  
- **Language** - All names should be in English.

- **Avoid Reserved Words** - Avoid naming objects with SQL reserved terms.

**Example** - Table name as a table name 


**Customer System & Enterprise System as crm & erp**

## Table Naming Convention

### ⛃ Naming Convention for Bronze Layer

- All names must start with the source system name, and table names must match their original names without renaming.

**sourcesystem_entity**

- **sourcesystem** - Name of the source system (e.g., **crm, erp**).

- **entity** - Exact table name from the source system.

**Example** - **crm_customer_info** → Customer information from the Customer System.

### ⛃ Naming Convention for Silver Layer

- All names must start with the source system name, and table names must match their original names without renaming.

**sourcesystem_entity**

- **sourcesystem** - Name of the source system (e.g., **crm, erp**).

- **entity** - Exact table name from the source system.

**Example** - **crm_customer_info** → Customer information from the Customer System.

### ⛃ Naming Convention for Gold Rules

- All names must use meaningful, business-aligned names for tables, starting with the category prefix.

**category_entity**

**category** - Describes the role of the table, such as

**Example**

- **dim** → dimension table

- **fact** → fact table

- **agg** → Aggregated Table

**entity** - Descriptive name of the table aligned with the business domain (e.g., customers, products, sales).

**Examples**

- **dim** → dim_customers, dim_product

- **fact** → fact_sales


## 💡 Data Architecture

The data structure outlines a **Medallion Architecture** **Bronze**, **Silver** & **Gold** layers.

<img width="851" height="448" alt="Database Layout" src="https://github.com/user-attachments/assets/fd12fdc9-d5b7-4c7b-ae96-37322a0353c1" />


1. **Bronze Layer** - Acts as a landing zone. It stores the data exactly as it appears in the source (like CSV Files).

2. **Silver Layer** - This is the "cleansing" stage where data is validated and made consistent.

3. **Gold Layer** - The final refined stage, optimized for performance and specific business use cases.

















































