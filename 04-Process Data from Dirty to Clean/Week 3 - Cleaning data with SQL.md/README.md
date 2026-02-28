# SQL vs Spreadsheets

SQL processes large amounts of data much faster than spreadsheets.

- Use **spreadsheets** when data already lives in Excel or Google Sheets.
- Use **SQL** when data is stored in a database.
- SQL handles large datasets efficiently.
- SQL is widely used in professional environments.
- Multiple team members can access the same database simultaneously.
- SQL queries can be tracked and versioned.

---

# What is SQL?

**Structured Query Language (SQL)** is used to communicate with databases.

There are different SQL dialects depending on the database system:
- MySQL
- PostgreSQL
- SQL Server
- BigQuery
- SQLite

Most analysts start with **Standard SQL**, then adjust syntax depending on the database.

---

# Basic SQL Commands

## SELECT and FROM

Used to retrieve data.

```sql
SELECT column_name
FROM table_name;
```

You must specify:
- The column(s)
- The table

---

## INSERT INTO

Used to add new records.

```sql
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);
```

---

## CREATE TABLE

Creates a new table.

```sql
CREATE TABLE IF NOT EXISTS table_name (
  column1 datatype,
  column2 datatype
);
```

Note: Running a SELECT query does not create a table.

---

## DROP TABLE

Removes a table.

```sql
DROP TABLE IF EXISTS table_name;
```

---

## DELETE

Removes rows from a table.

```sql
DELETE FROM table_name
WHERE condition;
```

---

## UPDATE

Modifies existing data.

```sql
UPDATE table_name
SET column = value
WHERE condition;
```

---

# Cleaning and Filtering with SQL

## DISTINCT

Removes duplicate values.

```sql
SELECT DISTINCT column_name
FROM table_name;
```

---

## String Functions

### LENGTH()

Checks number of characters.

```sql
SELECT LENGTH(column_name)
FROM table_name;
```

(Some databases use `LEN()` instead.)

---

### SUBSTR()

Extracts part of a string.

```sql
SELECT SUBSTR(column, start_position, number_of_characters)
FROM table_name;
```

---

### TRIM()

Removes extra spaces.

```sql
SELECT TRIM(column_name)
FROM table_name;
```

---

# Aggregate Functions

## MIN() and MAX()

```sql
SELECT MIN(column), MAX(column)
FROM table_name;
```

---

## COUNT()

```sql
SELECT COUNT(*)
FROM table_name;
```

---

# Data Type Conversion

## CAST()

Changes data type.

```sql
SELECT CAST(column AS data_type)
FROM table_name;
```

---

# Sorting

## ORDER BY

```sql
SELECT column
FROM table_name
ORDER BY column ASC;   -- or DESC
```

---

# Combining Data

## CONCAT()

Combines text fields.

```sql
SELECT CONCAT(column1, column2)
FROM table_name;
```

Useful for creating unique keys.

---

## COALESCE()

Returns first non-null value.

```sql
SELECT COALESCE(column1, column2)
FROM table_name;
```

Very useful for handling missing data.

---

# Key Takeaways

- SQL is powerful for large-scale analysis.
- It supports cleaning, transformation, and aggregation.
- It allows collaboration in database environments.
- Understanding Standard SQL makes adapting to dialects easier.
