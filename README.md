remove the markdown format and write as a readme file - # An-Employee-Management-System---Project
# Employee Management System (SQL Project)

## Problem Statement

Organizations manage large amounts of employee data including personal information, departments, salaries, attendance records, and performance reviews. When this data is not properly organized, it becomes difficult to retrieve useful information for decision-making.

This project solves that problem by creating a **relational SQL database** that organizes employee information into structured tables. The system allows managers and analysts to easily retrieve, analyze, and interpret employee data using SQL queries.

---

# Project Objectives

The main objectives of this project are:

- Design a relational database to manage employee data.
- Organize employee information across multiple related tables.
- Demonstrate the use of **primary keys and foreign keys**.
- Use SQL queries to retrieve and analyze employee data.
- Perform analytical queries such as filtering, sorting, and ranking employees.
- Demonstrate pagination and data retrieval techniques.

---

# Dataset Description

The dataset represents information typically stored in an organization's **Human Resources system**.

It includes the following categories of employee data:

- Employee personal information
- Departments within the company
- Job roles and salary ranges
- Salary history of employees
- Attendance records
- Employee performance reviews

This data is stored across **six structured tables** to maintain proper relationships and avoid redundancy.

---

# Database Schema

The database used in this project is called:
ProjectAss



The schema contains **six main tables**.

---

## 1. Jobs

Stores job roles available in the organization.

| Column | Description |
|------|-------------|
| JobID | Unique identifier for each job |
| JobTitle | Title of the job |
| MinSalary | Minimum salary range |
| MaxSalary | Maximum salary range |

---

## 2. Departments

Stores department information.

| Column | Description |
|------|-------------|
| DeptID | Unique department identifier |
| DeptName | Department name |
| Location | Department location |

---

## 3. Employees

Stores employee personal and job information.

| Column | Description |
|------|-------------|
| EmployeeID | Unique employee ID |
| FirstName | Employee first name |
| LastName | Employee last name |
| DateOfBirth | Employee birth date |
| Gender | Employee gender |
| Email | Employee email |
| PhoneNumber | Contact number |
| HireDate | Employment start date |
| JobID | Job reference |
| DepartmentID | Department reference |
| ManagerID | Employee's manager |
| Status | Employment status |

Status values include:

- Active
- Inactive
- On Leave

---

## 4. Salaries

Stores employee salary records.

| Column | Description |
|------|-------------|
| SalaryID | Salary record ID |
| EmployeeID | Employee reference |
| SalaryAmount | Salary value |
| FromDate | Start date |
| ToDate | End date |

---

## 5. Attendance

Stores daily attendance records.

| Column | Description |
|------|-------------|
| AttendanceID | Attendance record ID |
| EmployeeID | Employee reference |
| AttendanceDate | Date of attendance |
| Status | Present, Absent, Leave |
| CheckInTime | Clock-in time |
| CheckOutTime | Clock-out time |

---

## 6. Performance

Stores employee performance review records.

| Column | Description |
|------|-------------|
| PerformanceID | Performance record ID |
| EmployeeID | Employee reference |
| ReviewDate | Date of review |
| Rating | Performance score (1–5) |
| Comments | Manager comments |

---

### SQL Analysis
Several SQL queries were written to analyze the data and retrieve useful information. To mention a few:

---

## 1. Employee Full Name and Email
This query combines employee first and last names to generate a full name.
Screenshot
![Employee Names and Emails](screenshots/records of employee by their full names and email.JPG)

---
## active employees
There  are 61 active employees


---
## employee who are absent
There are 58 employee who are absent


---
## employees from the finance department who are still active
57 employees from the finance department are still active


---
## employee records who are paid above one hundred thousand
56 employee records are paid above one hundred thousand


---
## information about employees from the HR and Finance department
Here is a display of information about employees from the HR and Finance department


---
## Export records of employees aren’t active
54 employees aren’t active


---
## attendance records of employees who were present in attendance only in Jan 2026
53 emplouyees were in the Jan 2026 attendance records of employees who were present only in 

---
## records of employees from finance department and are still active
There is a records of 52 employees from finance department and are still active


---
## Order Employees by last name in alphabetical
Ordering Employees by last name alphabetical, '42', 'Owen', 'Adams', ranks top


---
## records of employees with the Highest Salaries First
There is a records of 50 employees that receives the Highest Salaries


---
## Unique Departments in the organization
There are 49 Unique Departments in the organization


---
Top 5 Performing Employees
This query identifies the highest-performing employees based on their rating.
The first name of the top 5 employees are mentioned below:
Sophia
Harper
Mia
Sophia
Harper

Screenshot
![Top 5 Performers](screenshots/Top 5 Performers.JPG)



---
3. Pagination Example (Next 5 Employees)
This query retrieves the next group of employees after the first five records.
The next five employees are listed below:
Mia
Sophia
Harper
Mia
Sophia
Screenshot
![Next 5 Employees](screenshots/Next 5 Employees (Pagination).JPG)




---
Key Business Insights
Based on the SQL analysis, the following insights were observed:
- The system successfully combines employee names and contact information for easy communication.
- The highest-performing employees received a rating of 5, indicating strong performance.
- Performance rankings can be easily generated using sorting and ordering queries.
- Pagination helps retrieve large datasets in smaller manageable groups.
- Joining tables allows employee data to be analyzed alongside performance records.



---
Tools Used
The following tools were used in this project:
MySQL Workbench – Database creation and query execution
SQL – Data analysis and manipulation
GitHub – Version control and project hosting
CSV Files – Exporting query results
Microsoft Excel – Viewing dataset outputs
Markdown – Documentation writing
Screenshot Tools – Capturing query results

Recommendations
Based on this project, the following improvements can enhance employee data analysis:
Implement automated dashboards using Power BI or Tableau.
Track employee attendance trends to detect absenteeism patterns.
Use SQL queries to identify salary gaps between job roles.
Monitor employee performance regularly to improve productivity.
Integrate the database with a web-based HR management system.


Author
Opeyemi Morakinyo
Business Intelligence Analyst
SQL | Excel | Power BI | Data Analysis
