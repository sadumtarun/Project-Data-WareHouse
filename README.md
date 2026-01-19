# Project-Data-WareHouse

This project involves the design and implementation of an Enterprise Data Warehouse (EDW) to integrate data from multiple operational source systems, including Customer Relationship Management (CRM) and Enterprise Resource Planning (ERP) platforms. The goal is to provide a single source of truth for business analytics, reporting, and decision-making.

The solution follows a layered data architecture (Bronze, Silver, Gold) to ensure data quality, scalability, and maintainability.

## 🗒️ Project Tasks  

- **Design Data Architecture**

- **Project Initilization**

- **Overarching Principles**

- **Building Bronze Layer**  


## 📐 Design Data Architecture

**Data Architecture**

<img width="600" height="450" alt="image" src="https://github.com/user-attachments/assets/2297cb89-2bb3-4173-955d-e0b83ce90698" />


**Database layout**

<img width="670" height="350" alt="image" src="https://github.com/user-attachments/assets/1a694dac-b1f7-40b6-aa49-1953e8411788" />


## 🚧 Project Initilization

- **Build Bronze Layer**

- **Build Sliver Layer**

- **Build Gold Layer**


## ✒️ Overarching Principles

### Table Naming Conventions

- **Naming Convention for Bronze Layer**

- **Naming Convention for Silver Layer**

- **Naming Convention for Gold Layer**

### Column Naming Conventions

- **Surrogate Keys**

- **Technical Columns**

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

- **agg** → agg_sales_week


## 🧱 Building Bronze Layer

### 🗪 Business Interaction with Clients / Source System Discussions

- **Business Environment and Ownership Roles**

- **System Architecture & Technology Stack**

- **Extract & Load**


### Business Environment and Ownership Roles

Who owns the data?

What Business Process it supports?

- Logisitcs, Customer Transcation, Supply Chain...

System & Data Documentation from the Source System

Data Model & Data Catalog

- Description of the columns and the tables


### System Architecture & Technology Stack

How the Source System is storing the data?

- AWS, Azure, SQL Server, Oracle

What are the Integration Tools / Connectivity Capabilities?

- How I'm going to get the data do the Source System offer APIs, Kafka or a direct connection.


### Extract & Load

Incremental vs Full Loads?

Data Range & Historical Data Scope?

- Complete Data or Specific Period Data...

Authentication & Authorization?

- Tokens, VPNs, SSH Keys...




