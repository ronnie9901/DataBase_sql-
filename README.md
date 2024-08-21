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

```sql
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("ROHAN",20,100000,"MANGER");
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("NARESH",21,190000,"CEO"); 
INSERT  INTO employeedata (name ,age,salary,role) VALUES ("SUMIT",20,190000,"DEV");

```

### Retrieve All Employee Information
```sql
SELECT * FROM employeesdata;
```

### Find Employees with a Specific Role
```sql
SELECT * FROM EmployeesData WHERE role = 'Manager';
```

### Search for Employees with Names Containing "An"
```sql
SELECT * FROM employeedata WHERE  name like 'Ro%';
```

### Find Employees Older than 30 and Earning More than $70,000
```sql
SELECT * FROM employeedata WHERE age > 20 AND salary > 70000;
```

### Change the Salary of an Employee with ID 3
```sql
UPDATE employeedata SET salary = 90000 WHERE id = 2;
```


## Delete All Employees with Age Less than 20
```sql
DELETE FROM employeedata WHERE age < 20;
```
