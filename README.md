# DataBase_sql-


# SQL

## Employee DBMS

### Setup
To set up the database, execute the following SQL script to create the employees table:

```sql
CREATE TABLE employeesdata (
    id INT,
    name TEXT,
    role TEXT,
    salary INT
    age INT,
);
```



### Add Multiple Employees with Selective Data

```
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("ROHAN",20,100000,"MANGER");
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("NARESH",21,190000,"CEO"); 
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("SUMIT",20,190000,"DEV");

```

 <img  height= "550" src="https://github.com/user-attachments/assets/f4c77cf7-2607-4a0b-a3b5-27dadc47296c"  />

     
### Retrieve All Employee Information
```
SELECT * FROM employeesdata;
```

### Find Employees with a Specific Role
```
SELECT * FROM EmployeesData WHERE name = 'NARESH';
```


 
### Search for Employees with Names Containing "Ro"
```sql
SELECT * FROM employeedata WHERE  name like 'Ro%';
```
 <img  height= "550" src="https://github.com/user-attachments/assets/9dba04e4-a92c-45ca-8d90-c95f4dc898db"  />


### Find Employees Older than 30 and Earning More than $70,000
```sql
SELECT * FROM employeedata WHERE age > 20 AND salary > 70000;
```

 <img  height= "550" src="https://github.com/user-attachments/assets/657fb27c-4ea6-490e-ace4-dc007316fdec"  />
 
### Change the Salary of an Employee with ID 2
```sql
UPDATE employeedata SET salary = 90000 WHERE id = 2;
```



## Delete All Employees with Age Less than 20
```sql
DELETE FROM employeedata WHERE age < 20;
```

 <img  height= "550" src="https://github.com/user-attachments/assets/33312882-9668-4f0e-8347-0b6e7f506a98"  />

