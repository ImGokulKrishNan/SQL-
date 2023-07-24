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
