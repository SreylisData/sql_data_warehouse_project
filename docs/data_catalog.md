# Data Catalog for Gold Layer


### **1. gold.dim_customers**
**• Purpose**: Stores customer details enriched with demographic and geographic data.

**• Columns**:
| Column Name | Data Type | Description |
| ------------- | ------------- | ------------- |
| customer_key | INT | Surrogate key uniquely identifying each customer record in the customers dimension table. |
| customer_id  | INT | Unique numerical identifier assigned to each customer. |
| customer_number | VARCHAR(50) | Alphanumeric identifier representing the customer, used for tracking and referencing. |
| first_name | VARCHAR(50) | The customer's first name. |
| last_name | VARCHAR(50) | The customer's ladt name. |
| country | VARCHAR(50) | The customer's country of residence (e.g. 'United Kingdom'). |
| marital_status | VARCHAR(50) | The customer's marital status (e.g. 'Single', 'Married'). |
| gender | VARCHAR(50) | The customer's gender (e.g. 'Female', 'Male', 'n/a'). |
| birthdate | DATE | The customer's date of birth, formatted as YYYY-MM-DD (e.g. 1995-01-28). |
| create_date | DATE | The date and time when the customer record was created in the system. |

---

### **2. gold.dim_products**
**• Purpose**: Stores customer details enriched with demographic and geographic data.

**• Columns**:
| Column Name | Data Type | Description |
| ------------- | ------------- | ------------- |
| product_key | INT | Surrogate key uniquely identifying each product record in the products dimension table. |
| product_id  | INT | ------------- |
| product_number | VARCHAR(50) |
| product_name | VARCHAR(50) |
| category_id | VARCHAR(50) |
| category | VARCHAR(50) |
| subcategory | VARCHAR(50) |
| maintenance | VARCHAR(50) |
| cost | INT |
| product_line | VARCHAR(50) |
| start_date | DATE |

---

### **3. gold.fact_sales**
**• Purpose**: Stores customer details enriched with demographic and geographic data.

**• Columns**:
| Column Name | Data Type | Description |
| ------------- | ------------- | ------------- |
| order_number | VARCHAR(50) | ------------- |
| product_key  | INT | ------------- |
| customer_key | INT |
| order_date | DATE |
| shipping_date | DATE |
| due_date | DATE |
| sales | INT |
| quantity | INT |
| price | INT |








