# Week 4 - SQL Practice

## Project Overview

This project contains SQL practice queries and assessment-style problems covering important SQL concepts using MySQL 8+.

It demonstrates database creation, data manipulation, joins, aggregate functions, subqueries, window functions, CTEs, and database views.

## Topics Covered

- NULL handling using IS NULL, COALESCE, and NULLIF
- Aggregate functions: COUNT, SUM, AVG, MIN, MAX
- GROUP BY and HAVING
- INNER JOIN, LEFT JOIN, and RIGHT JOIN
- FULL OUTER JOIN equivalent in MySQL
- CASE WHEN statements
- String functions
- Date and time functions
- DDL commands and constraints
- Scalar subqueries
- Correlated subqueries
- EXISTS and NOT EXISTS
- Window functions: RANK, DENSE_RANK, LAG, LEAD, NTILE
- Running totals and window frames
- Common Table Expressions (CTEs)
- Recursive CTEs
- UNION, INTERSECT, and EXCEPT
- ROLLUP
- CUBE equivalent in MySQL
- GROUPING SETS equivalent in MySQL
- Views
- Materialized-view concept using a snapshot table
- Assessment-style SQL questions

## Project Files

### 1. schema.sql

Creates the `week4_sql` database and the following tables:

- departments
- employees
- projects
- employee_projects
- customers
- orders

It defines primary keys, foreign keys, unique constraints, and other database relationships.

### 2. data.sql

Inserts sample records into the database tables, including employee details, department information, project assignments, customer details, and orders.

### 3. queries.sql

Contains SQL examples and assessment-style questions covering the Week 4 syllabus.

The queries demonstrate data retrieval, filtering, aggregation, joins, subqueries, window functions, and other SQL concepts.

## Database Relationships

- Each employee may belong to a department.
- Employees can report to managers.
- Departments can manage multiple projects.
- Employees and projects have a many-to-many relationship through employee_projects.
- Customers can place multiple orders.

## Technologies Used

- MySQL 8+
- SQL
- GitHub

## How to Run

Run the SQL files in the following order:

1. `schema.sql`
2. `data.sql`
3. `queries.sql`

### Using MySQL Workbench

1. Open MySQL Workbench.
2. Connect to your MySQL server.
3. Open `schema.sql` and execute it.
4. Open `data.sql` and execute it.
5. Open `queries.sql` and execute it.

Alternatively, use the MySQL command-line client:

```sql
SOURCE schema.sql;


Run these commands from the directory containing the files.

## Important Notes

- This project is designed for SQL practice and assessment preparation.
- The schema is intended for MySQL 8+.
- MySQL does not provide native `CREATE MATERIALIZED VIEW`, `CUBE`, or `GROUPING SETS` syntax; equivalent approaches are demonstrated.
- `INTERSECT` and `EXCEPT` require MySQL 8.0.31 or later.
- The schema script drops and recreates the `week4_sql` database. Back up any important data before executing it.

## Learning Outcomes

- Understand relational database design.
- Write SQL queries to retrieve and analyze data.
- Apply joins, aggregate functions, and subqueries.
- Use window functions and CTEs.
- Understand database constraints and relationships.
- Solve assessment-style SQL problems.
- Organize and maintain project files using GitHub.

## License

This project is intended for educational and learning purposes.
SOURCE data.sql;
SOURCE queries.sql;
