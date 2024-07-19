# Listing Databases

To display available databases, use the statement :

```sql
show databases;
```

Output :
```
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.01 sec)
```

# Creating Databases

Databases can be created using the `create database` statement.

```sql
create database learning;
```

Once created, the database should appear in the list of databases

```sql
show databases;
```

Output :
```
+--------------------+
| Database           |
+--------------------+
| information_schema |
| learning           |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
5 rows in set (0.00 sec)
```

We can also conditionally create a database if it doesn't already exist using:

```sql
create database if not exists learning;
```

# Selecting a Database

A database must be selected before it can be used. This is done with the `use` statement.

```sql
use learning;
```

All future statements like listing tables, creating tables, inserting or querying data will use the selected database.

# Deleting a Database

To delete a database, use `drop database`

```sql
drop database learning;
```

The database will no longer show up in the list of databases.

```sql
show databases;
```

Output :
```
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| sys                |
+--------------------+
4 rows in set (0.01 sec)
```

# Working with Tables


Create the tables for the Classic Models database. We will also insert some data along the way.

* Tables in a database can be listed using the `show tables` statement
* Tables are created using the `create table` statement
* Tables are deleted using the `drop table` statement
* You can view the structure of a table using the `describe` statement
* Data can be inserted into a table using the `insert into` statement

While creating tables, we specify a list of columns and the data type for each column. 

```sql
create table table_name (
    column1 datatype,
    column2 datatype,
    column3 datatype,
   ....
);
```