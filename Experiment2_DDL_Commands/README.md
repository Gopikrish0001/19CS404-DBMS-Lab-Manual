# Experiment 2: DDL Commands
# NAME  : GOPIKRISHNAN M
# REG NO: 212223043001



## AIM
To study and implement DDL commands and different types of constraints.

## THEORY

### 1. CREATE
Used to create a new relation (table).

**Syntax:**
```sql
CREATE TABLE (
  field_1 data_type(size),
  field_2 data_type(size),
  ...
);
```
### 2. ALTER
Used to add, modify, drop, or rename fields in an existing relation.
(a) ADD
```sql
ALTER TABLE std ADD (Address CHAR(10));
```
(b) MODIFY
```sql
ALTER TABLE relation_name MODIFY (field_1 new_data_type(size));
```
(c) DROP
```sql
ALTER TABLE relation_name DROP COLUMN field_name;
```
(d) RENAME
```sql
ALTER TABLE relation_name RENAME COLUMN old_field_name TO new_field_name;
```
### CONSTRAINTS
Constraints are used to specify rules for the data in a table. If there is any violation between the constraint and the data action, the action is aborted by the constraint. It can be specified when the table is created (using CREATE TABLE) or after it is created (using ALTER TABLE).
### 1. NOT NULL
When a column is defined as NOT NULL, it becomes mandatory to enter a value in that column.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) NOT NULL
);
```
### 2. UNIQUE
Ensures that values in a column are unique.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) UNIQUE
);
```
### 3. CHECK
Specifies a condition that each row must satisfy.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) CHECK (logical_expression)
);
```
### 4. PRIMARY KEY

```sql
INSERT INTO Products(ProductID,Name,Category,Price,Stock)
VALUES(106,'Fitness Tracker','Wearables',NULL,NULL);
INSERT INTO Products(ProductID,Name,Category,Price,Stock)
VALUES(107,'Laptop','Electronics',999.99,50);
INSERT INTO Products(ProductID,Name,Category,Price,Stock)
VALUES(108,'Wireless Earbuds','Accessories',NULL,100);
```

**Output:**

![image](https://github.com/user-attachments/assets/591defed-3658-4976-a479-3704104d7909)

**Question 8**

![image](https://github.com/user-attachments/assets/db29c91b-9692-462e-ac58-ad7c8a035391)

```sql
ALTER TABLE Companies ADD COLUMN designation varchar(50);
ALTER TABLE Companies ADD COLUMN net_salary number;
ALTER TABLE Companies ADD COLUMN dob date;
```

**Output:**

![image](https://github.com/user-attachments/assets/36f6e886-cdbc-40c1-937c-7d2559a0e7b3)

**Question 9**

![image](https://github.com/user-attachments/assets/04c55e88-d808-4cce-9f43-0a4b2daa2943)

```sql
CREATE TABLE jobs(
job_id INT,
job_title TEXT DEFAULT '',
min_salary INT DEFAULT 8000,
max_salary INT DEFAULT NULL);
```

**Output:**

![image](https://github.com/user-attachments/assets/4d67b31f-2b95-4c12-add8-b3054eb0448f)

**Question 10**

![image](https://github.com/user-attachments/assets/baedcb9b-7706-43c1-afd3-a0ca26f7c903)

```sql
ALTER TABLE Student_details ADD COLUMN Email VARCHAR(50);
ALTER TABLE Student_details ADD COLUMN MARKS INT DEFAULT 0;
```

**Output:**

![image](https://github.com/user-attachments/assets/e2dcd365-c733-4639-9d0d-e9db05b3eda1)


## RESULT
Thus, the SQL queries to implement different types of constraints and DDL commands have been executed successfully.








