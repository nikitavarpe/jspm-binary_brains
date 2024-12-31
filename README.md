# jspm-binary_brains
Repository for Inventory Management System

# Database Setup Script Documentation 
## Purpose
This script sets up a SQLite database ims.db for an Inventory Management System (IMS) with three tables: category, supplier, and product.

## Tables and Schema
### 1. category
**id:** Unique identifier (Primary Key, Auto-Increment).</br>
**name:** Category name (TEXT, Unique, Not Null).

### 2. supplier
**id:** Unique identifier (Primary Key, Auto-Increment).</br>
**name:** Supplier name (TEXT, Unique, Not Null).

### 3. product
**pid:** Unique identifier (Primary Key, Auto-Increment).</br>
**Category:** Foreign key referencing category(name) (TEXT, Not Null).</br>
**Supplier:** Foreign key referencing supplier(name) (TEXT, Not Null).</br>
**name:** Product name (TEXT, Unique, Not Null).</br>
**price:** Product price (REAL, Not Null).</br>
**qty:** Quantity in stock (INTEGER, Not Null).</br>
**status:** Product status (TEXT, Not Null).</br>
