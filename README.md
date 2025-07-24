# SQL Retail Database Project

A SQL-based relational database and analytics project built from a Kaggle dataset. This project involved designing a toy retail schema, populating six interrelated tables, and answering business-critical questions through advanced SQL queries.

---

## Tech Stack

- **SQL** (MySQL)
- **Python (Pandas)** – For data preprocessing and table creation
- **Data Source** – Kaggle: Toy Sales Data (custom cleaned and normalized)

---

##  Database Schema

The database includes the following tables:

- `CUSTOMER` – Customer demographics and region
- `PRODUCT` – Product details and MSRP
- `ORDER` – Order date and customer linkage
- `ORDERLINE` – Line items within each order
- `DEAL` – Deal size (e.g., Small, Medium, Large)
- `SHIPMENT` – Shipping status and territory

Each table was normalized and includes primary/foreign keys to maintain relational integrity.

---

##  Key Business Questions Answered

1. What is the total revenue generated from all orders?
2. Which are the top 3 product lines by sales?
3. What is the average order size?
4. Which customer-country pairs generate the most revenue?
5. What is the revenue loss between MSRP and actual price?

…and 6 more decision-critical queries including shipment patterns, deal sizes, and product performance by territory.

---

##  Process Overview

- Cleaned and split raw CSV into multiple relational tables using Python
- Added custom primary keys for consistency
- Handled import errors by converting data to JSON
- Converted and casted `FLOAT` and `DATETIME` fields in MySQL
- Ran analytical SQL queries to generate insights

---

## File Structure

| File | Description |
|------|-------------|
| `data_preprocessing.py` | Python script to clean and split data |
| `schema.sql` | MySQL table definitions |
| `populate_tables.sql` | Data import scripts |
| `analysis_queries.sql` | Business question queries |
| `ER_diagram.png` | Optional: Entity-Relationship Diagram |

---

