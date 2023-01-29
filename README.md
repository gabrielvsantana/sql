# SQL General Notes

## Table of Contents

- [1. Table Creation](#table-creation-and-deletion)
- [2. CRUD Example Operations](#crud-example-operations)

<br/>

---

# Table Creation and Deletion

## Table Creation

Creating a new table in a database can be done using the CREATE TABLE statement. It's important to note that the name of the table and the columns need to be defined along with the data types of each column. Here's an example of how to create a table called "employees":

```sql
CREATE TABLE employees (
    id INT PRIMARY KEY,
    first_name VARCHAR(255),
    last_name VARCHAR(255),
    email VARCHAR(255)
);
```

## Table Deletion

Deleting a table from a database can be done using the DROP TABLE statement. It's important to note that all the data inside of the table will be deleted permanently. Here's an example of how to delete the "employees" table:

```sql
DROP TABLE employees;
```

<br/>

---

# CRUD Example Operations

CRUD stands for Create, Read, Update, and Delete. These are the four basic operations that are performed on databases. In this section, we will go over an example of how to perform each of these operations using SQL.

## Create

The first operation is creating a new record in the database. In SQL, we use the INSERT INTO statement to do this. Here is an example of how to insert a new record into a table called customers:

```sql
INSERT INTO customers (first_name, last_name, email)
VALUES ('John', 'Doe', 'johndoe@example.com');
```

## Read

The second operation is reading data from the database. In SQL, we use the SELECT statement to do this. Here is an example of how to select all records from a table called customers:

```sql
SELECT * FROM customers;
```

## Update

The third operation is updating existing records in the database. In SQL, we use the UPDATE statement to do this. Here is an example of how to update the email of a customer with an ID of 1:

Copy code
UPDATE customers
```sql
UPDATE customers
SET email = 'newemail@example.com'
WHERE id = 1;
```

## Delete

The final operation is deleting records from the database. In SQL, we use the DELETE statement to do this. Here is an example of how to delete a customer with an ID of 1:

```sql
DELETE FROM customers
WHERE id = 1;
```

These are the basic CRUD operations that can be performed on a database using SQL. You can use these examples as a starting point for your own database operations.

<br/>

---