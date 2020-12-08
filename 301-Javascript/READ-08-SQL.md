# READ-08-SQL

## What is SQL

- Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database.

## Relational Databases

- A relational database represents a collection of related tables.

- Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns and any number of rows of data.

## SELECT STATEMENTS

- SELECT is basically a query. A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.

## SQL Lesson 2: Queries with constraints

- In order to filter certain results from being returned, we need to use a `WHERE` clause in the query.

- Checks each row to see if it should be included or not.

## SQL Lesson 4: Filtering and sorting Query results

- SQL provides a convenient way to discard rows that have a duplicate column value by using the `DISTINCT` keyword.

- SQL provides a way to sort your results by a given column in ascending or descending order using the `ORDER` BY clause.

- The `LIMIT` will reduce the number of rows to return, and the optional `OFFSET` will specify where to begin counting the number rows from.

- SELECT column, another_column, …
FROM mytable
WHERE condition(s)
ORDER BY column ASC/DESC
LIMIT num_limit OFFSET num_offset;

## SQL Lesson 13: Inserting rows

- When inserting data into a database, we need to use an `INSERT `statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. In general, each row of data you insert should contain values for every corresponding column in the table. You can insert multiple rows at a time by just listing them sequentially.

## SQL Lesson 14: Updating rows

- In addition to adding new data, a common task is to update existing data, which can be done using an `UPDATE` statement.

## SQL Lesson 15: Deleting rows

- you can use a `DELETE` statement to delete data from a table in the database.

## SQL Lesson 16: Creating tables

- The `CREATE TABLE` statement allows you to create a new database table.

## SQL Lesson 17: Altering tables

- `ALTER TABLE` statement to add, remove, or modify columns and table constraints.

## SQL Lesson 18: Dropping tables

- The `DROP TABLE` statement removes an entire table including all of its data and metadata.