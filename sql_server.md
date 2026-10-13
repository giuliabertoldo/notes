# INTRODUCTION TO SQL SERVER

* SQL native language for working with databases
* SQL Server relational database system developed by Microsoft
* T-SQL: Microsoft implementation of SQL (has additional functionalities)

## SELECT

* `SELECT` : what we want to retrieve from a table. For multiple columns, separate them with comma `(col1, col2)`

+ `FROM`: specifies the table 

* At the very end put ; 

* `SELECT TOP (5) artist` : 5 count

* `SELECT TOP (5) PERCENT artist` : 5%

* `SELECT DISTINCT`

* `SELECT *` : all columns

* `SELECT column AS col` : Alias

Example: Return half of the rows and all the columns
```sql
SELECT 
  TOP (50) PERCENT * 
FROM 
  eurovision;
```

## ORDER

* `ORDER BY`: placed after FROM. Multiple columns are separated by comma. 

* Default order is ascending. 

* `ORDER BY DESC` makes it descending (DESC should be placed after column name)

* You can order also using columns that do not appear in the SELECT statement. 

## WHERE

* After FROM 

* `WHERE points > 10` (<>, BETWEEN … AND (which is inclusive)

* `WHERE billing IS NULL / IS NOT NULL`

* When filtering strings, you need to wrap your value in 'single quotes'

* In Microsoft SQL Server dates are by default YYY-MM-DD and should be enclosed in ''


## MAIN

```sql
SELECT
FROM 
WHERE
ORDER BY
```







