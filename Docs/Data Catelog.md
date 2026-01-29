# Data Catalog - Gold Layer



### 1. **gold.dim_customers**

| Column Name      | Data Type     | Description                                                                                   |
|------------------|---------------|-----------------------------------------------------------------------------------------------|
| customer_key     | INT           | Surrogate key uniquely identifying each customer record in the dimension table.               |
| customer_id      | INT           | Unique numerical identifier assigned to each customer.                                        |
| customer_number  | NVARCHAR(50)  | Alphanumeric identifier representing the customer, used for tracking and referencing.         |
| first_name       | NVARCHAR(50)  | The customer's first name.                                                                    |
| last_name        | NVARCHAR(50)  | The customer's last name.                                                                     |
| country          | NVARCHAR(50)  | The country of residence for the customer                                                     |
| marital_status   | NVARCHAR(50)  | The marital status of the customer                                                           |
| gender           | NVARCHAR(50)  | The gender of the customer                                                                   |
| birthdate        | DATE          | The date of birth of the customer, formatted as YYYY-MM-DD (e.g., 2000-15-10).               |
| create_date      | DATE          | The date and time when the customer record was created in the system|
