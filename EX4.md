# Ex. No: 4 Creating Procedures using PL/SQL
# DATE:5.9.23
### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```
NAME: BHARATH K
Reg.no: 212222110006
```
```
SQL> create table employeee(empid number,empname varchar (20), dept varchar (10) ,salary number);

Table created.

SQL> create or replace procedure insert_employeee_data AS
     begin
     insert into employeee (empid,empname,dept,salary)
     values (1,'Bharath','MD',1000000);
     insert into employeee (empid,empname,dept,salary)
     values (2,'kavi','HR',500000);
     insert into employeee (empid,empname,dept,salary)
     values (3,'kishore','IT',200000);
     commit;
     end;
     /

Procedure created.

 begin
 insert_employeee_data;
 end;
 /

PL/SQL procedure successfully completed.

SQL> select * from employeee;
```
### Output:
![image](https://github.com/BharathCSEIOT/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/122793480/2fbe7ac3-c1d6-4e4b-bcfd-b7a455a95643)


### Result:
Hence the procedure using pl/sql is created successfully.
