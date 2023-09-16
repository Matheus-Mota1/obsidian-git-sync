
The command create is responsible to create databases and tables in SQL

# Create Database

Syntax to create a database:

```
CREATE DATABASE [database_name] IF NOT EXISTS;`
```

Example:

```SQL
CREATE DATABASE School IF NOT EXISTS;
```

You have to be careful creating a DATABASE because if it already exists will be overwrite.

# Creating Tables

```
CREATE TABLE [table_name](
Variable_name Type Constraints...
PRIMARY KEY(variable)
);
```

Related to [[Types and Constraints]].

Example:

```SQL
CREATE TABLE student (
	student_id INT AUTO_INCREMENT,
    name VARCHAR(20) NOT NULL,
    major VARCHAR(20) DEFAULT 'undecided'
    PRIMARY KEY(student_id)
);
```

Now that we created our table wee need to insert that into it through [[Insert and Delete]].