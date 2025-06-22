# SQL-Basics

## What is SQL?
SQL stands for Structured Query Language. It is used for storing and managing data in Relational Database Management System (RDBMS). It is a standard language for Relational DatabaseSystem. It enables a user to create, read, updateand delete relational databases and tables. All the RDBMS like MySQL, Informix, Oracle, MSAccess and SQL Server use SQL as their standarddatabase language. SQL allows users to query the database in a number of ways, using English-like statements.

## What are the SQL?
### SQL follows the following rules:
Structure query language is not case sensitive. Generally, keywords of SQL are written in uppercase. Statements of SQL are dependent on text lines. We can use a single SQL statement on one or multiple text line. Using the SQL statements, you can perform most of the actions in a database.  SQL depends on tuple relational calculus and relational algebra.

## What is SQL Process?
When an SQL command is executing for any RDBMS, then the system figure out the best way to carry out the request and the SQL engine determines that howto interpret the task. In the process, various components are included.These components can be optimization Engine, Queryengine, Query dispatcher, classic, etc. All the non-SQL queries are handled by the classic query engine, but SQL query engine won't handle logical files.

## What is SQL Process?
![image](https://github.com/user-attachments/assets/446e8676-6e52-47d5-ab86-9be4e8f27087)

## What is Advantages of SQL?
• High speed
• No coding needed
• Well defined standards
• Portability
• Interactive language
• Multiple data view

## What is SQL Datatype?
SQL Datatype is used to define the values that a column can contain. Every column is required to have a name and datatype in the database table.
![image](https://github.com/user-attachments/assets/42be3ef6-d034-4038-a8ab-454f55a0522e)

## SQL Commands
SQL commands are instructions. It is used tocommunicate with the database. It is also usedtoperform specific tasks, functions, and queries of data. SQL can perform various tasks like create a table, adddata to tables, drop the table, modify the table, setpermission for users.

## Types of SQL Commands
There are five types of SQL commands: DDL, DML, DCL, TCL, and DQL.
![image](https://github.com/user-attachments/assets/ab4da0af-df5c-4fe3-b14e-1cd65dd93811)

## Data Definition Language (DDL)
DDL changes the structure of the table like creating atable, deleting a table, altering a table, etc. All the command of DDL are auto-committed that means it permanently save all the changes in the database. Here are some commands that come under DDL:
 CREATE
 ALTER
 DROP
 TRUNCATE

### CREATE
CREATE : It is used to create a new table in the database.
Syntax : CREATE TABLE TABLE_NAME (COLUMN_NAME DATATYPES[,....]);
Example : CREATE TABLE EMPLOYEE(Name VARCHAR2(20), Email VARCHAR2(100), DOB DATE);

### DROP
DROP : It is used to delete both the structure and recordstored in the table.
Syntax : DROP TABLE ;
Example : DROP TABLE EMPLOYEE;

### ALTER
ALTER : It is used to alter the structure of the database. This changecould be either to modify the characteristics of an existing attribute or probably to add a new attribute. 
Syntax : ALTER TABLE table_name ADD column_name COLUMN-definition;
         ALTER TABLE MODIFY(COLUMN DEFINITION....);
Example : ALTER TABLE STU_DETAILS ADD(ADDRESS VARCHAR2(20));
          ALTER TABLE STU_DETAILS MODIFY (NAME VARCHAR2(20));

### TRUNCATE
TRUNCATE : It is used to delete all the rows from the table and freethe space containing the table. 
Syntax : TRUNCATE TABLE table_name;
Example : TRUNCATE TABLE EMPLOYEE;

## Data Manipulation Language (DML)
DML commands are used to modify the database. It isresponsible for all form of CHANGES in the database. The command of DML is not auto-committed that means it can't permanently save all the changes in thedatabase. They can be rollback. Here are some commands that come under DML:
 INSERT
 UPDATE
 DELETE

### INSERT
INSERT : The INSERT statement is a SQL query. It is used to insert data into the row of a table.
Syntax : INSERT INTO TABLE_NAME (col1, col2, col3,.... col N) VALUES (value1, value2, value3, .... valueN);
                                            OR
         INSERT INTO TABLE_NAME VALUES (value1, value2, value3, .... valueN);
Example : INSERT INTO XYZ (Author, Subject) VALUES ("Sonoo", "DBMS");

### UPDATE
UPDATE : This command is used to update or modify the value of acolumn in the table.
Syntax : UPDATE table_name SET [column_name1= value1,...column_nameN = valueN] [WHERE CONDITION]
Example : UPDATE students SET User_Name = 'Sonoo' WHERE Student_Id = '3'

## Data Control Language (DCL)
DCL commands are used to GRANT and TAKE BACK authority from any database user. Here are some commands that come under DCL:
 GRANT
 REVOKE

### GRANT
GRANT : It is used to give user access privileges to a database. 
Example : GRANT SELECT, UPDATE ON MY_TABLE TO SOME_USER, ANOTHER_USER;

### REVOKE
REVOKE : It is used to take back permissions from the user. 
Example : REVOKE SELECT, UPDATE ON MY_TABLE FROM USER1, USER2;

## Transaction Control Language (TCL)
TCL commands can only use with DML commands like INSERT, DELETE and UPDATE only.These operations are automatically committed in the database that's why they cannot be used while creatingtables or dropping them. Here are some commands that come under TCL:
 COMMIT
 ROLLBACK
 SAVEPOINT

### COMMIT
COMMIT : Commit command is used to save all the transactions tothe database.
Syntex : COMMIT;
Example: DELETE FROM CUSTOMERS WHERE AGE = 25;
         COMMIT;

### ROLLBACK
ROLLBACK : Rollback command is used to undo transactions that have not already been saved to the database. 
Syntax : ROLLBACK;
Example: DELETE FROM CUSTOMERS WHERE AGE = 25;
         ROLLBACK;

### SAVEPOINT
SAVEPOINT : It is used to roll thetransaction back to a certain point without rolling back the entire transaction. 
Syntax : SAVEPOINT SAVEPOINT_NAME;

## Data Query Language (DQL)
DQL is used to fetch the data from the database. It uses only one command : SELECT
a. SELECT : This is the same as the projection operation of relational algebra. It is used to select the attribute based on the condition described by WHERE clause. 
Syntax : SELECT expressions FROM TABLES WHERE conditions;
Example : SELECT emp_name FROM employee WHERE age > 20;

## SQL Operator
There are various types of SQL Operator:
![image](https://github.com/user-attachments/assets/57bd3183-1317-4a56-b7d1-886cd355d901)

## SQL Comparison Operators
![image](https://github.com/user-attachments/assets/a3668e74-5350-4ada-be74-377989c16521)

## SQL Arithmetic Operators
![image](https://github.com/user-attachments/assets/2b4b469a-7704-4f42-b9c5-4826bb32c6cd)
![image](https://github.com/user-attachments/assets/101bd490-8562-4d11-94a1-13278030c34e)

## SQL Logical Operators
![image](https://github.com/user-attachments/assets/2b149c9d-c7ad-4044-a051-2ed1c91cc020)





