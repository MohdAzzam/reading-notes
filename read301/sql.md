# SQL 

Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.

>There are many popular SQL databases including SQLite, MySQL, Postgres, Oracle and Microsoft SQL Server. All of them support the common SQL language standard, which is what this site will be teaching, but each implementation can differ in the additional features and storage types it supports.

--------------------------------------------------

## Relational databases

collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

-----------------------------------------------------

### SELECT queries

To retrieve data from a SQL database, we need to write `SELECT` statements
`queries` . A query in itself is just a statement which declares what data we are looking for, where to find it in the database, and optionally, how to transform it before it is returned.
`SELECT column, another_column, …FROM mytable;` to select specific column from the table
`SELECT * FROM mytable;` to select all data from the table 

------------------------

### Queries with constraints

Now we know how to select for specific columns of data from a table, but if you had a table with a hundred million rows of data, reading through all the rows would be inefficient and perhaps even impossible.

In order to filter certain results from being returned, we need to use a `WHERE` clause in the query. The clause is applied to each row of data by checking specific column values to determine whether it should be included in the results or not.

-----------------------------

### Filtering and sorting Query results 

Even though the data in a database may be unique, the results of any particular query may not be – take our Movies table for example, many different movies can be released the same year. In such cases, SQL provides a convenient way to discard rows that have a duplicate column value by using the `DISTINCT` keyword.

`SELECT DISTINCT column, another_column, …FROM mytable WHERE condition(s);`

`DISTINCT` keyword will `blindly` remove `duplicate rows,`

* Ordering results `ORDER BY column ASC/DESC;`
* Limiting results to a subset `LIMIT num_limit OFFSET num_offset;`


--------------------------
What is a Schema?  
> the structure of each table, and the datatypes that each column of the table can contain.

### Inserting rows 

When inserting data into a database, we need to use an `INSERT` statement, which declares which table to write into, the columns of data that we are filling, and one or more rows of data to insert. In general, each row of data you insert should contain values for every corresponding column in the table. You can insert multiple rows at a time by just listing them sequentially.

`INSERT INTO mytable VALUES (value_or_expr, another_value_or_expr, …),(value_or_expr_2, another_value_or_expr_2, …),…;`

------------------------------------

### Updating rows 
 `INSERT` statement, you have to specify exactly which table, columns, and rows to update. In addition, the data you are updating has to match the data type of the columns in the table schema.

UPDATE mytable
`SET column = value_or_expr,  other_column = another_value_or_expr, …WHERE condition;`

----------------------------

### Deleting rows 
When you need to delete data from a table in the database, you can use a DELETE statement, which describes the table to act on, and the rows of the table to delete through the WHERE clause.

`DELETE FROM mytable WHERE condition;`

If you decide to leave out the WHERE constraint, then all rows are removed, which is a quick and easy way to clear out a table completely (if intentional).

----------------------------------

### Creating tables

`CREATE TABLE IF NOT EXISTS mytable ( column DataType TableConstraint DEFAULT default_value, another_column DataType TableConstraint DEFAULT default_value,…);`

CREATE TABLE movies (
    id INTEGER PRIMARY KEY,
    title TEXT,
    director TEXT,
    year INTEGER, 
    length_minutes INTEGER
);

--------------------------------------

### Altering tables
 As your data changes over time, SQL provides a way for you to update your corresponding tables and database schemas by using the ALTER TABLE statement to add, remove, or modify columns and table constraints.

* Adding columns ` ALTER TABLE mytable ADD column DataType OptionalTableConstraint  DEFAULT default_value;`
* Removing columns `ALTER TABLE mytable DROP column_to_be_deleted;`
* Renaming the table `ALTER TABLE mytable RENAME TO new_table_name;`


------------------------------------------------

### Dropping tables
In some rare cases, you may want to remove an entire table including all of its data and metadata, and to do so, you can use the DROP TABLE statement, which differs from the DELETE statement in that it also removes the table schema from the database entirely.

`Drop table statement DROP TABLE IF EXISTS mytable;`

 
