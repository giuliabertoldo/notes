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

* `WHERE .... AND ....` : for multiple conditions and where neceaasry use parenthese. Other operators: `OR `, `IN`, `LIKE 'a%'`, 

Example:
```sql
SELECT song
FROM songlist
WHERE 
    artist = 'Green Day' 
    AND (
        release_year = 1994
        OR release_year > 2000
    )
```

* When filtering strings, you need to wrap your value in 'single quotes'

* In Microsoft SQL Server dates are by default YYY-MM-DD and should be enclosed in ''


## MAIN

```sql
SELECT
FROM 
WHERE
ORDER BY
```

## AGGREGATING DATA

* Calculate total amount in a column: `SELECT SUM(col) AS colsum_alias`

* Count number of rows in a column: `SELECT COUNT(col) AS colcount_alias`

* Count number of unique values ina. column: `SELECT COUNT(DISTINCT col) as unique_count_affected`

* Minimum, maximum, average value in a column:`SELECT MIN() ... AS / MAX() ... AS / AVG()...AS `


## WORKING WITH STRINGS

* `SELECT LEN(col) AS ...` : length of a column

*  `SELECT LEFT(col, 5) AS first_five_left`: extract a number of characters from beginning of a string 

* `SELECT RIGHT(col, 5) AS last_five_right`: extract a number of characters from end of a string 

* `SELECT CHARINDEX('_', url) AS char_location`: find underscore location in url column

* `SELECT SUBSTRING(col, 12, 2) AS target_section`: select two characters after 12 characters

* `SELECT REPLACE(col, '_', '-') AS replace_with_hyphen`

## GROUPING AND HAVING












