# SQL Queries: Classic Models Sales Database

Eight SQL queries answering business questions on a retail sales database (a model-car company), covering data modification, filtering, aggregation, and inner and outer joins.

## Questions and Results

| # | Question | Technique | Result |
|---|---|---|---|
| 1 | Delete the unused `Boats` product line, then count `productlines` rows | `DELETE`, `COUNT` | **7** rows (from 8) |
| 2 | Count order lines with product code starting `S18` and price above 150 | `LIKE`, filtering | **26** |
| 3 | Top 3 countries by number of customers | `GROUP BY`, `ORDER BY`, `LIMIT` | **USA (35), Germany (13), France (12)** |
| 4 | Average credit limit for Singapore | `AVG` | **67,233.33** |
| 5 | Total amount paid by "Euro+ Shopping Channel" | `INNER JOIN`, `SUM` | **715,738.98** |
| 6 | Month with the highest total payments, and that total | `MONTH()`, `GROUP BY` | **December**, 1,645,923.26 (summed across all years) |
| 7 | Average credit limit of customers handled by employees in the Tokyo office | 3-table `INNER JOIN` | **83,900.00** |
| 8 | Customer who paid the lowest total amount | `LEFT JOIN`, `HAVING` | **Boards & Toys Co.** (7,918.60) |

## Database
The queries use a sales database named `company` with these tables: `offices`, `employees`, `customers`, `orders`, `orderdetails`, `payments`, `productlines` and `products`. The database and its data are **not included** in this repository.

## How to Run
1. Create and load the `company` database in MySQL.
2. Open `classic_models_queries.sql` in MySQL Workbench and run the queries one at a time.

## Tech Stack
SQL (MySQL) · MySQL Workbench

## Author
**Anju Kanwar**
