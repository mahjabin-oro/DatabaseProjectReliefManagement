# Relief Management Database System

A relational database for **managing disaster-relief operations**. It tracks donors, donated goods, victims, relief distribution, branches, wards and workers. It was built in **Oracle SQL and PL/SQL** for a database systems course.

---

## What it models

| Table | What it stores |
|---|---|
| `branch` | Relief organisation branches |
| `wards` | Areas or wards each branch serves |
| `donor` | People and organisations who donate |
| `goods` | Types of relief goods and their stock |
| `donation` | Donations received (who gave what, and how much) |
| `victim` | Affected people who need help |
| `relief` | Relief given out to victims |
| `job` / `worker` | Volunteers and staff, and their roles |

## Database features shown

- **Schema design** with primary keys, foreign keys and constraints (`tables.sql`)
- **Sample data** for testing (`insert_data.sql`)
- **Queries**: joins, subqueries, aggregate functions, grouping and filtering (`allLabs.sql`)
- **PL/SQL** (`plsql.sql`):
  - A **function** that calculates the remaining stock after relief is given out
  - A **stored procedure** that updates the total goods
  - A **trigger** that checks donation data before it is inserted or updated
  - A **view** of completed donations

## Tech stack

Oracle Database · SQL · PL/SQL

## How to use

Run the scripts in this order in Oracle SQL*Plus or SQL Developer:

1. `tables.sql.txt`: create the schema
2. `insert_data.sql.txt`: load the sample data
3. `allLabs.sql.txt` and `plsql.sql.txt`: run the queries, functions, procedures and triggers
