# BDD200 – Project 1 (Oracle SQL) 
## Overview
This project builds an Oracle SQL database for a simple retail system inspired by No Frills.  
It includes:
- ERD (with PK/FK, required fields, crow’s foot relationships)
- Data Dictionary
- Table Creation Scripts (CREATE TABLE)
- Data Insertion Scripts (INSERT INTO)
- SQL Report (SELECT / JOIN / VIEW queries)
- Demo video (optional link)

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

