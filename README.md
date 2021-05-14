# dbmsbasic
SQL Commands: DML, DDL, DCL, TCL, DQL with Query Example
What is SQL?
SQL is a database language designed for the retrieval and management of data in a relational database.

SQL is the standard language for database management. All the RDBMS systems like MySQL, MS Access, Oracle, Sybase, Postgres, and SQL Server use SQL as their standard database language. SQL programming language uses various commands for different operations. We will learn about the like DCL, TCL, DQL, DDL and DML commands in SQL with examples.

In this SQL commands in DBMS tutorial, you will learn:

What is SQL?
Why Use SQL?
Brief History of SQL
Types of SQL
What is DDL?
What is Data Manipulation Language?
What is DCL?
What is TCL?
What is DQL?
Why Use SQL?
Here, are important reasons for using SQL

It helps users to access data in the RDBMS system.
It helps you to describe the data.
It allows you to define the data in a database and manipulate that specific data.
With the help of SQL commands in DBMS, you can create and drop databases and tables.
SQL offers you to use the function in a database, create a view, and stored procedure.
You can set permissions on tables, procedures, and views.
Brief History of SQL
Here, are important landmarks from the history of SQL:

1970 - Dr. Edgar F. "Ted" Codd described a relational model for databases.
1974 - Structured Query Language appeared.
1978 - IBM released a product called System/R.
1986 - IBM developed the prototype of a relational database, which is standardized by ANSI.
1989- First ever version launched of SQL
1999 - SQL 3 launched with features like triggers, object-orientation, etc.
SQL2003- window functions, XML-related features, etc.
SQL2006- Support for XML Query Language
SQL2011-improved support for temporal databases
Types of SQL
Here are five types of widely used SQL queries.

Data Definition Language (DDL)
Data Manipulation Language (DML)
Data Control Language(DCL)
Transaction Control Language(TCL)
Data Query Language (DQL)
Types of SQL
Types of SQL

Let see each of them in detail:

What is DDL?
Data Definition Language helps you to define the database structure or schema. Let's learn about DDL commands with syntax.

Five types of DDL commands in SQL are:

CREATE
CREATE statements is used to define the database structure schema:

Syntax:

CREATE TABLE TABLE_NAME (COLUMN_NAME DATATYPES[,....]); 
For example:

Create database university;
Create table students;
Create view for_students;
DROP
Drops commands remove tables and databases from RDBMS.

Syntax

DROP TABLE ;
For example:

Drop object_type object_name;
Drop database university;
Drop table student;
ALTER
Alters command allows you to alter the structure of the database.

Syntax:

To add a new column in the table

ALTER TABLE table_name ADD column_name COLUMN-definition; 
To modify an existing column in the table:

ALTER TABLE MODIFY(COLUMN DEFINITION....);  
For example:

Alter table guru99 add subject varchar; 
TRUNCATE:
This command used to delete all the rows from the table and free the space containing the table.

Syntax:

TRUNCATE TABLE table_name;  
Example:

TRUNCATE table students;
What is Data Manipulation Language?
Data Manipulation Language (DML) allows you to modify the database instance by inserting, modifying, and deleting its data. It is responsible for performing all types of data modification in a database.

There are three basic constructs which allow database program and user to enter data and information are:

Here are some important DML commands in SQL:

INSERT
UPDATE
DELETE
INSERT:
This is a statement is a SQL query. This command is used to insert data into the row of a table.

Syntax:

INSERT INTO TABLE_NAME  (col1, col2, col3,.... col N)  
VALUES (value1, value2, value3, .... valueN);  
Or 
INSERT INTO TABLE_NAME    
VALUES (value1, value2, value3, .... valueN);    
For example:

INSERT INTO students (RollNo, FIrstName, LastName) VALUES ('60', 'Tom', Erichsen');
UPDATE:
This command is used to update or modify the value of a column in the table.

Syntax:

UPDATE table_name SET [column_name1= value1,...column_nameN = valueN] [WHERE CONDITION]   
For example:

UPDATE students    
SET FirstName = 'Jhon', LastName= 'Wick' 
WHERE StudID = 3;
DELETE:
This command is used to remove one or more rows from a table.

Syntax:

DELETE FROM table_name [WHERE condition];  
For example:

DELETE FROM students 
WHERE FirstName = 'Jhon';
What is DCL?
DCL (Data Control Language) includes commands like GRANT and REVOKE, which are useful to give "rights & permissions." Other permission controls parameters of the database system.

Examples of DCL commands:
Commands that come under DCL:

Grant
Revoke
Grant:
This command is use to give user access privileges to a database.

Syntax:

GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;  
For example:

GRANT SELECT ON Users TO'Tom'@'localhost;
Revoke:
It is useful to back permissions from the user.

Syntax:

REVOKE privilege_nameON object_nameFROM {user_name |PUBLIC |role_name}
For example:

REVOKE SELECT, UPDATE ON student FROM BCA, MCA;  
What is TCL?
Transaction control language or TCL commands deal with the transaction within the database.

Commit
This command is used to save all the transactions to the database.

Syntax:

Commit;
For example:

DELETE FROM Students  
WHERE RollNo =25;  
COMMIT;  
Rollback
Rollback command allows you to undo transactions that have not already been saved to the database.

Syntax:

ROLLBACK;  
Example:

DELETE FROM Students  
WHERE RollNo =25;  
SAVEPOINT
This command helps you to sets a savepoint within a transaction.

Syntax:

SAVEPOINT SAVEPOINT_NAME;
Example:

SAVEPOINT RollNo;
What is DQL?
Data Query Language (DQL) is used to fetch the data from the database. It uses only one command:

SELECT:
This command helps you to select the attribute based on the condition described by the WHERE clause.

Syntax:

SELECT expressions    
FROM TABLES    
WHERE conditions;  
For example:

SELECT FirstName  
FROM Student  
WHERE RollNo > 15;  
Summary:
SQL is a database language designed for the retrieval and management of data in a relational database.
It helps users to access data in the RDBMS system
In the year 1974, the term Structured Query Language appeared
Five types of SQL queries are 1) Data Definition Language (DDL) 2) Data Manipulation Language (DML) 3) Data Control Language(DCL) 4) Transaction Control Language(TCL) and, 5) Data Query Language (DQL)
Data Definition Language(DDL) helps you to define the database structure or schema.
Data Manipulation Language (DML) allows you to modify the database instance by inserting, modifying, and deleting its data.
DCL (Data Control Language) includes commands like GRANT and REVOKE, which are useful to give "rights & permissions."
Transaction control language or TCL commands deal with the transaction within the database.
Data Query Language (DQL) is used to fetch the data from the database.
 
