# SQL-
SQL Data type:

Number (P, S): 

DDL

create 
	create table data(a varchar2(3),b number(3));

alter is using only table already exsting table

	Add	
		alter table data
		add(new number(3));  to use multiple add columns
	Modify
		alter table data
		modify(new number(4));	to use multiple columns
	Drop
		alter table data+
		drop column a,b,c;      to use multiple columns
	Rename		alter table data
		rename a to abc;			only one column
Drop
	Drop table abc;
	drop table abc purge;			not to retrive table
	
Flashback 
flashback table student to before drop;
Truncate
	
	Truncate table table-name --> Removes all values from table,

Rename 
	rename abc to abd;
		
DML
•	Insert
			insert into table-name values(a number(2),b varchar2(21));
			insert into table (a,b,c) values(1,2,3);
•	Update
			update data set a=11;						  --> one row
			update data set a=11 where acc=12;			  --> paricular row 
			update data set a=11 where acc in (11,22,33); --> muptiple row update using IN-->special operator
			
•	Delete
			deleate table b;
			delete table a;
			
•	Merge

DQL/DRL
	Select
TCL
	Commit
	Savepoint
	Rollabck
DCL
grand /revoke

Operator
	Arithmatic operator 
		Add +
		sub -
		multiply *
		div 
	Commaration Operator
		= EQUAL
		< LESS THAN
		> GRATER THAN
		<= LESS THAN OR EQUAL
		>= GRATER THAN OR EQUAL
		<> NOT EQUAL
lOGICAL OPERATOR
AND true condition  
OR one condition true 
NOT  
SPECIAL OPERATOR

IS 
BETWEEN


LIKE
IS NULL
NOT IS 
NOT BETWEEN
NOT LIKE
NOT IS NULL


SELECTC QUERY FLOW

SQL FUNCTION
	NUMBER FUNCTION
	CHARACTER FUNCTION
	DATE FUNCTION
	GROUP FUNCTION

9i & JOINS

SQL CONSTRAINS

SET OPERATOR

ANALYTICAL FUNCTION

ROWNUM ,ROWID

VIEW IN SQL

HANDLING NULL VALUES

INDEXING IN  SQL

TYPE OF INDEXING

DECODE FUNCTION

DATE CONVERSION FUNCTION

SUB QUERY 



create table sample;
alter table sample
add(new number(10,ad varchar2(12));

alter table sample 
modify(new number(12),ad varchar2(123));

alter table sample 
drop column a,b,c;

alter table sample 
rename sample to asd;


truncate table sample;

flashback table sample before drop;

DML

insert table sample values (new,dad,asd,f,4234)

update table sample set= 123 where acc=234;

merge

delete table sample;

DQL/DRL
select

DCL
Revoke
grant
TCL
Rollback
commit
savepoint

lOGICAL OPERATOR
AND true condition  
OR one condition true 
NOT  
SPECIAL OPERATOR

IS 
BETWEEN
LIKE
IS NULL
NOT IS 
NOT BETWEEN
NOT LIKE
NOT IS NULL


select
from 
where
groupby
order by

CTE
WITH cte_name (column_names)   
AS (query)     
SELECT * FROM cte_name;    
1) What is SQL?
SQL stands for the Structured Query Language. It is the standard language used to maintain the relational database and perform many different data manipulation operations on the data. SQL was initially invented in 1970. It is a database language used for database creation, deletion, fetching and modifying rows, etc. sometimes, it is pronounced as 'sequel.' We can also use it to handle organized data comprised of entities (variables) and relations between different entities of the data.

2) When SQL appeared?
SQL first appeared in 1974. It is one of the most used languages for maintaining the relational database. In 1986, SQL became the standard of the American National Standards Institute (ANSI) and ISO (International Organization for Standardization) in 1987.

3) What are the usages of SQL?
SQL is responsible for maintaining the relational data and the data structures present in the database. Some of the common usages are given below:

To execute queries against a database
To retrieve data from a database
To inserts records in a database
To updates records in a database
To delete records from a database
To create new databases
To create new tables in a database
To create views in a database
To perform complex operations on the database.
4) Does SQL support programming language features?
SQL refers to the Standard Query Language. Therefore, it is true that SQL is a language but does not actually support the programming language. It is a common language that doesn't have a loop, conditional statements, and logical operations. It cannot be used for anything other than data manipulation. It is a command language to perform database operations. The primary purpose of SQL is to retrieve, manipulate, update, delete, and perform complex operations like joins on the data present in the database.

5) What are the subsets of SQL?
The following are the four significant subsets of the SQL:

Data definition language (DDL): It defines the data structure that consists of commands like CREATE, ALTER, DROP, etc.
Data manipulation language (DML): It is used to manipulate existing data in the database. The commands in this category are SELECT, UPDATE, INSERT, etc.
Data control language (DCL): It controls access to the data stored in the database. The commands in this category include GRANT and REVOKE.
Transaction Control Language (TCL): It is used to deal with the transaction operations in the database. The commands in this category are COMMIT, ROLLBACK, SET TRANSACTION, SAVEPOINT, etc.
AD
6) What is the purpose of DDL Language?
DDL stands for Data definition language. It is the subset of a database that defines the data structure of the database when the database is created. For example, we can use the DDL commands to add, remove, or modify tables. It consists of the following commands: CREATE, ALTER and DELETE database objects such as schema, tables, indexes, view, sequence, etc.

Example

CREATE TABLE Students  
(  
Roll_no INT,  
Name VARCHAR(45),  
Branch VARCHAR(30),  
);  
7) What is the purpose of DML Language?
Data manipulation language makes the user able to retrieve and manipulate data in a relational database. The DML commands can only perform read-only operations on data. We can perform the following operations using DDL language:

Insert data into the database through the INSERT command.
Retrieve data from the database through the SELECT command.
Update data in the database through the UPDATE command.
Delete data from the database through the DELETE command.
Example

INSERT INTO Student VALUES (111, 'George', 'Computer Science')  
8) What is the purpose of DCL Language?
Data control language allows users to control access and permission management to the database. It is the subset of a database, which decides that what part of the database should be accessed by which user at what point of time. It includes two commands, GRANT and REVOKE.

GRANT: It enables system administrators to assign privileges and roles to the specific user accounts to perform specific tasks on the database.

REVOKE: It enables system administrators to revoke privileges and roles from the user accounts so that they cannot use the previously assigned permission on the database.

Example

GRANT * ON mydb.Student TO javatpoint@localhsot;  
9) What are tables and fields in the database?
A table is a set of organized data in the form of rows and columns. It enables users to store and display records in the structure format. It is similar to worksheets in the spreadsheet application. Here rows refer to the tuples, representing the simple data item, and columns are the attribute of the data items present in a particular row. Columns can categorize as vertical, and Rows are horizontal.

Fields are the components to provide the structure for the table. It stores the same category of data in the same data type. A table contains a fixed number of columns but can have any number of rows known as the record. It is also called a column in the table of the database. It represents the attribute or characteristics of the entity in the record.

Example
AD

Table: Student

Field: Stud_rollno, Stud_name, Date of Birth, Branch, etc.

10) What is a primary key?
A primary key is a field or the combination of fields that uniquely identify each record in the table. It is one of a special kind of unique key. If the column contains a primary key, it cannot be null or empty. A table can have duplicate columns, but it cannot have more than one primary key. It always stores unique values into a column. For example, the ROLL Number can be treated as the primary key for a student in the university or college.

SQL Interview Questions and Answers
We can define a primary key into a student table as follows:

CREATE TABLE Student (    
    roll_number INT PRIMARY KEY,    
    name VARCHAR(45),     
);    
To read more information, click here.
AD

11) What is a foreign key?
The foreign key is used to link one or more tables together. It is also known as the referencing key. A foreign key is specified as a key that is related to the primary key of another table. It means a foreign key field in one table refers to the primary key field of the other table. It identifies each row of another table uniquely that maintains the referential integrity. The primary key-foreign key relationship is a very crucial relationship as it maintains the ACID properties of the database sometimes. It also prevents actions that would destroy links between the child and parent tables.

We can define a foreign key into a table as follows:

CONSTRAINT constraint_name]    
    FOREIGN KEY [foreign_key_name] (col_name, ...)    
    REFERENCES parent_tbl_name (col_name,...)    
To read more information, click here.

12) What is a unique key?
A unique key is a single or combination of fields that ensure all values stores in the column will be unique. It means a column cannot stores duplicate values. This key provides uniqueness for the column or set of columns. For example, the email addresses and roll numbers of student's tables should be unique. It can accept a null value but only one null value per column. It ensures the integrity of the column or group of columns to store different values into a table.

We can define a foreign key into a table as follows:

CREATE TABLE table_name(    
    col1 datatype,    
    col2 datatype UNIQUE,    
    ...    
);  
To read more information, click here.

13) What is the difference between a primary key and a unique key?
The primary key and unique key both are essential constraints of the SQL. The main difference among them is that the primary key identifies each record in the table. In contrast, the unique key prevents duplicate entries in a column except for a NULL value. The following comparison chart explains it more clearly:

Primary Key	Unique Key
The primary key act as a unique identifier for each record in the table.	The unique key is also a unique identifier for records when the primary key is not present in the table.
We cannot store NULL values in the primary key column.	We can store NULL value in the unique key column, but only one NULL is allowed.
We cannot change or delete the primary key column values.	We can modify the unique key column values.
To read more information, click here.

14) What is a Database?
A database is an organized collection of data that is structured into tables, rows, columns, and indexes. It helps the user to find the relevant information frequently. It is an electronic system that makes data access, data manipulation, data retrieval, data storing, and data management very easy. Almost every organization uses the database for storing the data due to its easily accessible and high operational ease. The database provides perfect access to data and lets us perform required tasks.

The following are the common features of a database:

Manages large amounts of data
Accurate
Easy to update
Security
Data integrity
Easy to research data
15) What is meant by DBMS?
DBMS stands for Database Management System. It is a software program that primarily functions as an interface between the database and the end-user. It provides us the power such as managing the data, the database engine, and the database schema to facilitate the organization and manipulation of data using a simple query in almost no time. It is like a File Manager that manages data in a database rather than saving it in file systems. Without the database management system, it would be far more difficult for the user to access the database's data.

The following are the components of a DBMS:

Software
Data
Procedures
Database Languages
Query Processor
Database Manager
Database Engine
Reporting
16) What are the different types of database management systems?
The database management systems can be categorized into several types. Some of the important lists are given below:

Hierarchical databases (DBMS)
Network databases (IDMS)
Relational databases (RDBMS
Object-oriented databases
Document databases (Document DB)
Graph databases
ER model databases
NoSQL databases
17) What is RDBMS?
RDBMS stands for Relational Database Management System. It is a database management system based on a relational model. It facilitates you to manipulate the data stored in the tables by using relational operators. RDBMS stores the data into the collection of tables and links those tables using the relational operators easily whenever required. Examples of relational database management systems are Microsoft Access, MySQL, SQL Server, Oracle database, etc.

18) What is Normalization in a Database?
Normalization is used to minimize redundancy and dependency by organizing fields and table of a database.

There are some rules of database normalization, which is commonly known as Normal From, and they are:

First normal form(1NF)
Second normal form(2NF)
Third normal form(3NF)
Boyce-Codd normal form(BCNF)
Using these steps, the redundancy, anomalies, inconsistency of the data in the database can be removed.

19) What is the primary use of Normalization?
Normalization is mainly used to add, delete or modify a field that can be made in a single table. The primary use of Normalization is to remove redundancy and remove the insert, delete and update distractions. Normalization breaks the table into small partitions and then links them using different relationships to avoid the chances of redundancy.

20) What are the disadvantages of not performing database Normalization?
The major disadvantages are:

The occurrence of redundant terms in the database causes the waste of space in the disk.

Due to redundant terms, inconsistency may also occur. If any change is made in the data of one table but not made in the same data of another table, then inconsistency will occur. This inconsistency will lead to the maintenance problem and effects the ACID properties as well.

21) What is an inconsistent dependency?
An Inconsistent dependency refers to the difficulty of getting relevant data due to a missing or broken path to the data. It leads users to search the data in the wrong table, resulting in an error as an output.

22) What is Denormalization in a Database?
Denormalization is a technique used by database administrators to optimize the efficiency of their database infrastructure. The denormalization concept is based on Normalization, which is defined as arranging a database into tables correctly for a particular purpose. This method allows us to add redundant data into a normalized database to alleviate issues with database queries that merge data from several tables into a single table. It adds redundant terms into the tables to avoid complex joins and many other complex operations.

Denormalization doesn't mean that normalization will not be done. It is an optimization strategy that takes place after the normalization process.

23) What are the different types of SQL operators?
Operators are the special keywords or special characters reserved for performing particular operations. They are also used in SQL queries. We can primarily use these operators within the WHERE clause of SQL commands. It's a part of the command to filters data based on the specified condition. The SQL operators can be categorized into the following types:

Arithmetic operators: These operators are used to perform mathematical operations on numerical data. The categories of this operators are addition (+), subtraction (-), multiplication (*), division (/), remainder/modulus (%), etc.
Logical operators: These operators evaluate the expressions and return their results in True or False. This operator includes ALL, AND, ANY, ISNULL, EXISTS, BETWEEN, IN, LIKE, NOT, OR, UNIQUE.
Comparison operators: These operators are used to perform comparisons of two values and check whether they are the same or not. It includes equal to (=), not equal to (!= or <>), less than (<), greater than (>), less than or equal to (<=), greater than or equal to (>=), not less than (!<), not greater than (!>), etc.
Bitwise operators: It is used to do bit manipulations between two expressions of integer type. It first performs conversion of integers into binary bits and then applied operators such as AND (& symbol), OR (|, ^), NOT (~), etc.
Compound operators: These operators perform operations on a variable before setting the variable's result to the operation's result. It includes Add equals (+=), subtract equals (-=), multiply equals (*=), divide equals (/=), modulo equals (%=), etc.
String operators: These operators are primarily used to perform concatenation and pattern matching of strings. It includes + (String concatenation), += (String concatenation assignment), % (Wildcard), [] (Character(s) matches), [^] (Character(s) not to match), _ (Wildcard match one character), etc.
24) What is a view in SQL?
A view is a database object that has no values. It is a virtual table that contains a subset of data within a table. It looks like an actual table containing rows and columns, but it takes less space because it is not present physically. It is operated similarly to the base table but does not contain any data of its own. Its name is always unique. A view can have data from one or more tables. If any changes occur in the underlying table, the same changes reflected in the views also.

SQL Interview Questions and Answers
The primary use of a view is to implement the security mechanism. It is the searchable object where we can use a query to search the view as we use for the table. It only shows the data returned by the query that was declared when the view was created.

We can create a view by using the following syntax:

CREATE VIEW view_name AS  
SELECT column_lists FROM table_name  
WHERE condition;  
25) What is an Index in SQL?
An index is a disc structure associated with a table or view that speeds up row retrieval. It reduces the cost of the query because the query's high cost will lead to a fall in its performance. It is used to increase the performance and allow faster retrieval of records from the table. Indexing reduces the number of data pages we need to visit to find a particular data page. It also has a unique value meaning that the index cannot be duplicated. An index creates an entry for each value which makes it faster to retrieve data.

For example: Suppose we have a book which carries the details of the countries. If you want to find out information about India, why will you go through every page of that book? You could directly go to the index. Then from the index, you can go to that particular page where all the information about India is given.

26) What are the different types of indexes in SQL?
SQL indexes are nothing more than a technique of minimizing the query's cost. The higher the query's cost, the worse the query's performance. The following are the different types of Indexes supported in SQL:

Unique Index
Clustered Index
Non-Clustered Index
Bit-Map Index
Normal Index
Composite Index
B-Tree Index
Function-Based Index
27) What is the unique index?
UNIQUE INDEX is used to enforce the uniqueness of values in single or multiple columns. We can create more than one unique index in a single table. For creating a unique index, the user has to check the data in the column because the unique indexes are used when any column of the table has unique values. This indexing does not allow the field to have duplicate values if the column is unique indexed. A unique index can be applied automatically when a primary key is defined.

We can create it by using the following syntax:

CREATE UNIQUE INDEX index_name    
ON table_name (index_column1, index_column2,...);  
Example

CREATE TABLE Employee(      
    ID int AUTO_INCREMENT PRIMARY KEY,       
    Name varchar(45),     
    Phone varchar(15),    
    City varchar(25),   
);  
Suppose we want to make a Phone column as a unique index. We can do this like below:

CREATE UNIQUE INDEX index_name_phone ON Employee (Phone);    
To read more information, click here.

28) What is clustered index in SQL?
A clustered index is actually a table where the data for the rows are stored. It determines the order of the table data based on the key values that can sort in only one direction. Each table can have only one clustered index. It is the only index, which has been automatically created when the primary key is generated. If many data modifications needed to be done in the table, then clustered indexes are preferred.

To read more information, click here.

29) What is the non-clustered index in SQL?
The indexes other than PRIMARY indexes (clustered indexes) are called non-clustered indexes. We know that clustered indexes are created automatically when primary keys are generated, and non-clustered indexes are created when multiple joins conditions and various filters are used in the query. The non-clustered index and table data are both stored in different places. It cannot be able to alter the physical order of the table and maintains the logical order of data.

The purpose of creating a non-clustered index is for searching the data. Its best example is a book where the content is written in one place, and the index is at a different place. We can create 0 to 249 non-clustered indexes in each table. The non-clustered indexing improves the performance of the queries which use keys without assigning the primary key.

30) What are the differences between SQL, MySQL, and SQL Server?
The following comparison chart explains their main differences:

SQL	MySQL	SQL Server
SQL or Structured Query Language is useful for managing our relational databases. It is used to query and operate the database.	MySQL is the popular database management system used for managing the relational database. It is a fast, scalable, and easy-to-use database.	SQL Server is an RDBMS database system mainly developed for the Windows system to store, retrieve, and access data requested by the developer.
SQL first appeared in 1974.	MySQL first appeared on May 23, 1995.	SQL Server first appeared on April 24, 1989.
SQL was developed by IBM Corporation.	MySQL was developed by Oracle Corporation.	SQL Server was developed by Microsoft Company.
SQL is a query language for managing databases.	MySQL is database software that uses SQL language to conduct with the database.	SQL Server is also a software that uses SQL language to conduct with the database.
SQL has no variables.	MySQL can use variables constraints and data types.	SQL Server can use variables constraints and data types.
SQL is a programming language, so that it does not get any updates. Its commands are always fixed and remain the same.	MySQL is software, so it gets frequent updation.	SQL Server is also software, so it gets frequent updation.
