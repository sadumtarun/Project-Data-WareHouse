## ✒️ Overarching Principles

### Rules

- **Naming conventions** - Use snake_case, separating words with underscores (`_`) and lowercase letters.
- **Language** - All names should be in English.
- **Avoid Reserved Words** - Avoid naming objects with SQL reserved terms.
**Example** - Table name as a table name 


**Customer System & Enterprise System as crm & erp**

## Table Naming Convention

### ⛃ Bronze Layer Rules

- All names must start with the source system name, and table names must match their original names without renaming.

**`<sourcesystem>_<entity>`**
- `<sourcesystem>` - Name of the source system (e.g., `crm`, `erp`).
- `<entity>` - Exact table name from the source system.

**Example** - `<crm_customer_info>` → Customer information from the Customer System.

### ⛃ Silver Layer Rules

- All names must start with the source system name, and table names must match their original names without renaming.

`<sourcesystem_entity>`
- `<sourcesystem>` - Name of the source system (e.g., `crm`, `erp`).
- `<entity>` - Exact table name from the source system.

**Example** -  `crm_customer_info` → Customer information from the Customer System.

### ⛃ Gold Layer Rules

- All names must use meaningful, business-aligned names for tables, starting with the category prefix.

`<category_entity>`
`category` - Describes the role of the table, such as

**Example**

- `dim` → dimension table
- `fact` → fact table


`<entity>` - Descriptive name of the table aligned with the business domain (e.g., customers, products, sales).

**Examples**

- `dim` → dim_customers, dim_product
- `fact` → fact_sales


### **Surrogate Keys**  

- All primary keys in dimension tables must use the suffix `_keys`.

- **`<table_name>_keys`**

  - `<table_name>` - Refers to the name of the table or entity the key belongs to.  
  - `_keys` - A suffix indicating that this column is a surrogate key.

  - Example: `customer_keys` → Surrogate key in the `dim_customers` table.
 

  ## **Stored Procedure**

- All stored procedures used for loading data must follow the naming pattern:
- **`load_<layer>`**.
  
  - `<layer>` - Represents the layer being loaded, such as `bronze`, `silver`, or `gold`.
  - Example
  
    - `load_bronze` → Stored procedure for loading data into the Bronze layer.
    - `load_silver` → Stored procedure for loading data into the Silver layer.
