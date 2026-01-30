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
