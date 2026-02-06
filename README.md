# BDD200 – Project 1 (Oracle SQL) | Group 6 – No Frills Retail Database

## Overview
This project builds an Oracle SQL database for a simple retail system inspired by No Frills.  
It includes:
- ERD (with PK/FK, required fields, crow’s foot relationships)
- Data Dictionary
- Table Creation Scripts (CREATE TABLE)
- Data Insertion Scripts (INSERT INTO)
- SQL Report (SELECT / JOIN / VIEW queries)
- Demo video (optional link)

## Team & Responsibilities
**Group 6 Members:**
- Thi Yen Nhi Huynh: PROJECT_STORES, PROJECT_CUSTOMERS
- Tai Nguyen: PROJECT_PRODUCTS, PROJECT_EMPLOYEES
- Trinh Trong Tin Le: PROJECT_ORDERS, PROJECT_ORDER_ITEMS

## Database Entities
- PROJECT_STORES
- PROJECT_CUSTOMERS
- PROJECT_PRODUCTS
- PROJECT_EMPLOYEES
- PROJECT_ORDERS
- PROJECT_ORDER_ITEMS

## Relationships (High Level)
- PROJECT_STORES (1) → (many) PROJECT_EMPLOYEES via store_id
- PROJECT_STORES (1) → (many) PROJECT_ORDERS via store_id
- PROJECT_CUSTOMERS (1) → (many) PROJECT_ORDERS via customer_id
- PROJECT_ORDERS (1) → (many) PROJECT_ORDER_ITEMS via order_id
- PROJECT_PRODUCTS (1) → (many) PROJECT_ORDER_ITEMS via product_id

## How to Run (Oracle SQL Developer)
1. Open **SQL Worksheet**
2. Run scripts in this order:
   1) `scripts/01_create_tables.sql`
   2) `scripts/02_insert_data.sql`
   3) `scripts/03_views.sql`
   4) `scripts/04_queries.sql`
3. Verify tables: expand **Tables** in the connection.
4. Take screenshots of:
   - Columns tab
   - Constraints tab
   - Data tab (showing >= 20 rows where required)

## Files Included
### /docs
- ERD diagram screenshots (with header: student name, course code, section)
- Data Dictionary tables
- SQL query output screenshots

### /scripts
- CREATE TABLE scripts
- INSERT scripts
- VIEW scripts
- SELECT/JOIN query scripts

## Notes
- Uses `SET DEFINE OFF;` to prevent substitution prompts when inserting strings.
- All constraints include PK/FK, NOT NULL, UNIQUE, and CHECK rules where required.

## License
For educational use only (Seneca – BDD200).

