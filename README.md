# Lab Performance 04 – Constraints (MySQL)

## Course Information
- **Course Code:** CSE 210  
- **Course Title:** Database Management Systems  
- **Lab Title:** Lab Performance 04 – Constraints  
- **Section:** 242D3  

---

## Task Description
This Task implements the given Entity Relationship Diagram (ERD) using **MySQL**.  
The database includes four tables: `COUNTRY`, `DEPARTMENT`, `EMPLOYEE`, and `FOLDER`.

The implementation follows proper database design principles including:
- Primary Keys
- Foreign Keys
- NOT NULL constraints
- Additional constraints such as `UNIQUE` and `ENUM`

---

## ERD Overview
The database schema is based on the following relationships:

- One **Country** can have multiple **Departments**
- One **Department** can have multiple **Employees**
- One **Employee** can have multiple **Folders**

---

## Tables Implemented
1. **COUNTRY**
   - CountryId (Primary Key)
   - CountryName (UNIQUE, NOT NULL)
   - Continent
   - Currency

2. **DEPARTMENT**
   - DepartmentId (Primary Key)
   - DeptName
   - CountryId (Foreign Key)

3. **EMPLOYEE**
   - EmpID (Primary Key)
   - EmpName
   - DeptId (Foreign Key)

4. **FOLDER**
   - FolderId (Primary Key)
   - EmpId (Foreign Key)
   - AccessType (ENUM: READ, WRITE, FULL)

---

## Constraints Used
- **Primary Key (PK)**
- **Foreign Key (FK)**
- **NOT NULL**
- **UNIQUE**
- **ENUM**

---

## Data Insertion
- Each table contains **5 sample records**
- Data insertion follows **referential integrity rules**
- No constraint violations occur during insertion

---

## How to Run the Project

1. Open **MySQL Command Line Client** or **MySQL Workbench**
2. Create a database (optional if already included in SQL file)
3. Run the SQL file:
   ```sql
   SOURCE lab_performance_04.sql;
