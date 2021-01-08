# Experiment-8

Implementation of various aggregate functions in SQL

-- Questions:

-- 1. Create a table Employee with following specifications.

--    Code, name, DOB, designation, salary

-- 2. Insert values into the table

-- 3. Display sum of salaries from the table employee where designation is clerk.

-- 4. Describe the maximum salary value from the table employee.

-- 5. Display average salary of employees

-- 6. Describe the minimum salary value from the table

-- 7. Display the total number of employees.

#1 

CREATE TABLE Employee(

    code CHAR(6) PRIMARY KEY,

    name VARCHAR(80),

    dob date,

    designation VARCHAR(100),

    salary FLOAT

);

#2

INSERT INTO Employee (code, name, dob, designation, salary)

VALUES

('emp101','Jack ','2000-10-08','General Manager',50000.25),

('emp108','Aravind','1998-10-15','Product Manager',50000.50),

('emp110','Sathya','1992-05-06','Clerk',25000),

('emp132','Varun','2001-05-05','Clerk',15000.85);

#3

SELECT SUM(salary) FROM Employee WHERE designation='Clerk';

#4

SELECT MAX(salary) FROM Employee;

#5

SELECT AVG(salary) FROM Employee;

#6

SELECT MIN(salary) FROM Employee;

#7

SELECT COUNT(*) FROM Employee;






output:

#3
SUM(salary)
40000.849609375
#4
MAX(salary)

50000.5
#5
AVG(salary)

35000.39990234375
#6
MIN(salary)

15000.849609375
#7
COUNT(*)

4






 
   
 


























