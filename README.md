# 🏫 School Database SQL Project

This project demonstrates the design and implementation of a simple relational database system for a school using SQL.

## 🗂️ Project Overview

The `School` database consists of two tables:

- `students`
- `teachers`

Each table includes appropriate constraints to maintain data integrity and enforce real-world business logic, such as:
- Unique and required phone numbers for emergency contact.
- Unique emails for students and teachers.
- Primary key IDs.
- Constraints reflecting graduation year and department tracking.

## 🧰 Tools Used

- MySQL / PostgreSQL
- SQL

## 📌 Table Schemas

### `students`
| Column          | Type         | Constraints                  |
|-----------------|--------------|------------------------------|
| student_id      | INT          | PRIMARY KEY                  |
| first_name      | VARCHAR(50)  | NOT NULL                     |
| last_name       | VARCHAR(50)  | NOT NULL                     |
| homeroom_number | INT          |                              |
| phone           | VARCHAR(20)  | NOT NULL, UNIQUE             |
| email           | VARCHAR(100) | UNIQUE                       |
| graduation_year | INT          |                              |

### `teachers`
| Column          | Type         | Constraints                  |
|-----------------|--------------|------------------------------|
| teacher_id      | INT          | PRIMARY KEY                  |
| first_name      | VARCHAR(50)  | NOT NULL                     |
| last_name       | VARCHAR(50)  | NOT NULL                     |
| homeroom_number | INT          |                              |
| department      | VARCHAR(50)  |                              |
| email           | VARCHAR(100) | NOT NULL, UNIQUE             |
| phone           | VARCHAR(20)  | NOT NULL, UNIQUE             |

## ✅ Sample Data Inserted

- **Student**: Mark Watney, Class of 2035  
- **Teacher**: Jonas Salk, Biology Department  

## 📄 SQL Script

All schema creation and data insertion can be found in [`school_database.sql`](./school_database.sql).


