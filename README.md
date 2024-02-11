# Windows Functions for Advanced SQL on Windows

This repository provides a collection of SQL scripts and examples showcasing the use of advanced SQL window functions on Windows, specifically focusing on the analysis of the New York Airbnb Open Data available on Kaggle. The scripts cover importing CSV files into tables, along with advanced SQL queries using `OVER`, `PARTITION BY`, `ROW_NUMBER`, `RANK` & `DENSE_RANK`, and `LEAD` and `LAG` functions.

## Table of Contents

1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [Importing CSV File into Table](#importing-csv-file-into-table)
4. [Advanced SQL Queries](#advanced-sql-queries)
    - [OVER Clause](#over-clause)
    - [PARTITION BY](#partition-by)
    - [ROW_NUMBER](#row-number)
    - [RANK & DENSE_RANK](#rank--dense_rank)
    - [LEAD and LAG](#lead-and-lag)
5. [Example Usage](#example-usage)
6. [Contributing](#contributing)
7. [License](#license)

## Introduction

Window functions in SQL provide a powerful way to perform calculations across a set of rows related to the current row. This repository aims to demonstrate the use of these functions to analyze the New York Airbnb Open Data available on Kaggle. The examples provided here are focused on the Windows platform.

## Getting Started

To get started, follow these steps:

1. Clone this repository to your local machine.
2. Make sure you have a SQL Server instance installed on your Windows system.
3. Create a new database and configure the connection details in the scripts.

## Importing CSV File into Table

The first step is to import the New York Airbnb Open Data CSV file into a table in your SQL Server database. Use the provided script in the [import_csv.sql](import_csv.sql) file to achieve this. Modify the script according to your database configuration.

```sql
-- Example Usage:
-- Run the following query in SQL Server Management Studio (SSMS)
-- Make sure to modify the file path and database details accordingly

USE YourDatabaseName;

-- Run the import script
:r import_csv.sql;
```

## Advanced SQL Queries

### OVER Clause

The `OVER` clause is used to define a window or set of rows for a window function. See [over_clause.sql](over_clause.sql) for examples.

### PARTITION BY

The `PARTITION BY` clause divides the result set into partitions to which the window function is applied independently. Check [partition_by.sql](partition_by.sql) for usage examples.

### ROW_NUMBER

The `ROW_NUMBER` function assigns a unique number to each row within a partition of a result set. See [row_number.sql](row_number.sql) for implementations.

### RANK & DENSE_RANK

The `RANK` and `DENSE_RANK` functions assign ranks to rows based on the values in specified columns. Refer to [rank_dense_rank.sql](rank_dense_rank.sql) for usage examples.

### LEAD and LAG

The `LEAD` and `LAG` functions access data from subsequent or previous rows in a result set. Explore [lead_lag.sql](lead_lag.sql) for illustrations.

