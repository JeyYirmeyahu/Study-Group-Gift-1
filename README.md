SQL Employee Database Analysis Project

📌 Project Overview

This project demonstrates foundational SQL querying techniques using an employee database.
The tasks cover schema creation, CSV data importation, data filtering, logical conditions, and pattern matching using SQL queries.

The project is ideal for beginners learning how to work with relational databases and perform data analysis using SQL.


---

🛠️ Database Setup & Data Import

Step 1: Create a New Schema

Open MySQL Workbench

Select Create a New Schema

Provide a schema name and apply changes


Step 2: Import CSV Data

Right-click the created schema

Select Table Data Import Wizard

Locate and select the CSV file

Choose a table name

Continue clicking Next

Click Finish

Refresh the schema to display the imported table



---

📂 Employee Database Queries

🔹 Level 1: Basic Filtering

Display All Employees

SELECT * 
FROM employees.employees;

Employees Earning ₦120,000 and Above

SELECT first_name, last_name, salary
FROM employees
WHERE salary >= 120000;

Retrieve Employee Details Using Employee Number

SELECT DISTINCT *
FROM employees
WHERE employment_number = 1005;

Employees Working in the IT Department

SELECT DISTINCT first_name, last_name, gender, department
FROM employees
WHERE department = 'IT';


---

🔹 Level 2: Smart Logic Queries

Female Employees in the Finance Department

SELECT *
FROM employees
WHERE gender = 'Female'
AND department = 'Finance';

Employees Earning Between ₦70,000 and ₦90,000

SELECT DISTINCT *
FROM employees
WHERE salary BETWEEN 70000 AND 90000;

Employees Who Are Not Currently Active

SELECT *
FROM employees
WHERE employment_status <> 'Active';


---

🔹 Level 3: Pattern Matching & Conditional Queries

Employees with “Manager” in Their Job Title

SELECT *
FROM employees
WHERE job_title LIKE '%Manager%';

Employees in Sales, Marketing, or Operations

SELECT *
FROM employees
WHERE department IN ('Sales', 'Marketing', 'Operations');

Employees Whose First Name Starts with “A”

SELECT *
FROM employees
WHERE first_name LIKE 'A%';

Male Employees Working in Sales or IT

SELECT *
FROM employees
WHERE gender = 'Male'
AND (department = 'Sales' OR department = 'IT');

Male Employees Hired After January 1, 2015

SELECT *
FROM employees
WHERE gender = 'Male'
AND hire_date > '2015-01-01';

Male Employees Earning More Than ₦80,000

SELECT *
FROM employees
WHERE gender = 'Male'
AND salary > 80000;


---

📊 Skills Demonstrated

Database Schema Creation

CSV Data Importation

SQL Data Filtering

Logical Operators (AND, OR, BETWEEN)

Pattern Matching with LIKE

Conditional Queries

Data Retrieval Techniques

Query Optimization Basics



---

🚀 Tools Used

MySQL Workbench

SQL

CSV Dataset



---

📖 Learning Outcome

Through this project, I gained hands-on experience in:

Writing efficient SQL queries

Importing and managing datasets

Filtering and analyzing employee records

Applying logical and conditional SQL statements

Working with real-world employee datasets



---

📬 Connect With Me

If you found this project helpful or would like to collaborate on data analytics projects, feel free to connect with me.

💼 Data Analyst

📊 SQL | Excel | SPSS | R

📈 Data Cleaning • Analysis • Visualization
