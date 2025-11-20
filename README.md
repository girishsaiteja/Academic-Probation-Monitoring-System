The CGPA Monitoring System is a PL/SQL-based academic performance tracking tool that automates CGPA calculation, updates student status, and identifies students who fall below the minimum academic threshold.
This project demonstrates strong practical use of SQL, PL/SQL functions, triggers, and relational database design.

🛠️ Tech Stack:
SQL & PL/SQL
Oracle Database
Functions & Stored Procedures
Triggers (AFTER INSERT)
Cursors (for reporting)
ERD-style relational table design

🗂️ Database Structure
Tables Created

STUDENTS
Stores student ID and name.

MARKS
Stores marks for six subjects for each student.

GPA_INFO
Stores calculated CGPA and a “Flagged” status (Y/N).

🚀 Key Features
✅ 1. Automated CGPA Calculation
A PL/SQL function calculates CGPA using marks from six subjects and returns a numeric value.

✅ 2. Trigger for Automatic Status Update
An AFTER INSERT trigger runs whenever new marks are entered, calculates CGPA, and updates:
CGPA value
Flagged status ("Y" if CGPA < 4, "N" otherwise)

✅ 3. Academic Risk Identification
The system automatically identifies low-performing students and stores them for follow-ups and academic support.

✅ 4. Clean and Scalable Design
The relational structure allows the project to be extended to more subjects, semesters, or academic rules.

🧮 Core PL/SQL Logic (Summary)

Function: Calculates CGPA from six subjects.

Trigger: Automates calculation and updates GPA_INFO after each student’s marks are inserted.

Cursor: Used to generate structured output reports for flagged students.
