## relational databases and SQL

# SELECT is a keyword used in SQL (Structured Query Language) to retrieve data from one or more tables in a database. A SELECT query allows you to specify the columns of data you want to retrieve, as well as the conditions under which you want to retrieve them.


# SELECT column1, column2, ...
# FROM table_name
 # WHERE condition;
# The SELECT statement specifies which columns you want to retrieve from the table. You can select all columns by using *. The FROM clause specifies which table you want to retrieve data from. The WHERE clause is optional, but allows you to filter the data based on a specific condition.

# For example, the following query retrieves all columns from the "customers" table where the "country" column is equal to "USA":

# SELECT *
# FROM customers
# WHERE country = 'USA';
# task1

## Queries with constraints are used to filter the data that is returned by the query.
# For example, the following query retrieves all rows from the "employees" table where the "salary" column is greater than $50,000:

# SELECT *
# FROM employees
# WHERE salary > 50000;
# Other types of constraints include:
# AND and OR operators: These operators are used to combine multiple constraints in a single query. For example, the following query retrieves all rows from the "employees" table where the "salary" column is greater than $50,000 and the "department" column is equal to "Marketing":

# SELECT *
# FROM employees
# WHERE salary > 50000 AND department = 'Marketing';
# IN operator: This operator is used to match a value against a list of possible values.
# For example, the following query retrieves all rows from the "employees" table where the "department" column is either "Marketing" or "Sales":

# SELECT *
# FROM employees
# WHERE department IN ('Marketing', 'Sales');
# LIKE operator: This operator is used to match a value against a pattern.
# For example, the following query retrieves all rows from the "employees" table where the "last_name" column starts with "Smi":



## The basic syntax for an ALTER TABLE statement is as follows:
# ALTER TABLE table_name
# ADD column_name datatype constraints;

# ALTER TABLE table_name
# RENAME TO new_table_name;

# ALTER TABLE table_name
# DROP COLUMN column_name;


# The basic syntax for an DROP TABLE statement is as follows:
# DROP TABLE table_name;

[screen shot for lessons](./sql/)
