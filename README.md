# Complaint Management System

A MySQL-based Complaint Management System designed to manage customer complaints efficiently. The system allows users to register complaints, assigns them to departments and employees, tracks complaint status, logs complaint history, and collects customer feedback after resolution.

---

## Project Overview

The Complaint Management System helps organizations streamline the complaint-handling process from registration to resolution.

It supports:

- Complaint registration.
- Complaint assignment.
- Complaint status tracking.
- Complaint history logging.
- Customer feedback collection.
- Employee performance analysis.
- Department-wise complaint reports.

---

## Technologies Used

- MySQL 8.0.
- MySQL Workbench.
- SQL.
- ER Diagram.
- Relational Database Design.

---

## Database Schema

### Database Name

```sql
CREATE DATABASE complaint_management;
USE complaint_management;
```

---

## Database Tables

| Table | Description |
|---|---|
| Users | Stores customer/user information. |
| Employees | Stores employee details. |
| Departments | Stores department information. |
| Priority | Stores complaint priority levels. |
| ComplaintStatus | Stores complaint status values. |
| Complaints | Stores complaint details. |
| ComplaintHistory | Stores complaint status history. |
| Feedback | Stores customer feedback. |

---

## Entity Relationships

- One User can raise many Complaints.
- One Department can handle many Complaints.
- One Employee can manage many Complaints.
- One Complaint can have multiple History records.
- One Complaint can receive Feedback after resolution.

---

## Features

- User complaint registration.
- Department-wise complaint management.
- Employee assignment.
- Priority management.
- Complaint status tracking.
- Complaint history logging.
- Feedback collection.
- SQL reporting.
- Performance analysis.

---

## SQL Concepts Used

### Basic SQL
- SELECT
- WHERE
- ORDER BY
- GROUP BY
- DISTINCT
- LIMIT
- Aggregate Functions

### Intermediate SQL
- INNER JOIN
- LEFT JOIN
- HAVING
- Subqueries
- Date Functions
- GROUP BY Analysis

### Advanced SQL
- Common Table Expressions (CTE)
- Window Functions
- RANK()
- Running Totals
- Nested Queries
- Performance Reports

---

## Sample Reports

The project includes SQL queries to generate:

- Department-wise complaint count.
- Employee performance report.
- Average resolution time.
- Monthly complaint summary.
- Customer feedback analysis.
- Critical priority complaints.
- Complaint status report.
- Top-performing employees.
- Complaint history report.

---

## Database Relationships

```text
Users (1) --------< Complaints

Departments (1) --< Employees

Departments (1) --< Complaints

Employees (1) ---< Complaints

Priority (1) ----< Complaints

ComplaintStatus (1) --< Complaints

Complaints (1) --< ComplaintHistory

ComplaintStatus (1) --< ComplaintHistory

Complaints (1) --< Feedback

Users (1) -------< Feedback
```

---

## Project Workflow

```text
Customer
     │
     ▼
Register Complaint
     │
     ▼
Complaint Created
     │
     ▼
Assign Department
     │
     ▼
Assign Employee
     │
     ▼
Update Complaint Status
     │
     ▼
Complaint History Updated
     │
     ▼
Complaint Resolved
     │
     ▼
Customer Feedback Submitted
```

---

## Folder Structure

```text
Complaint-Management-System/
│
├── SQL/
│   ├── Database.sql
│   ├── Tables.sql
│   ├── Insert_Data.sql
│   ├── Beginner_Queries.sql
│   ├── Intermediate_Queries.sql
│   ├── Advanced_Queries.sql
│   ├── Stored_Procedures.sql
│   └── Triggers.sql
│
├── ER_Diagram.png
├── Relationship_Diagram.png
├── Project_Report.pdf
└── README.md
```

---

## Learning Outcomes

This project demonstrates practical knowledge of:

- Database design.
- Relational database management.
- SQL query writing.
- Data analysis.
- Window functions.
- CTEs.
- Aggregate functions.
- Joins.
- Database relationships.
- Report generation.

---

## Future Enhancements

- Authentication system.
- Admin dashboard.
- Email notifications.
- Complaint attachments.
- Role-based access control.
- REST API integration.
- Frontend web application.
- Complaint analytics dashboard.

---

## Author

NandhaKumar V  
BCA Graduate  
Frontend & Java Full Stack Developer

GitHub: [Nandhakumar-007](https://github.com/Nandhakumar-007)

---

## License

This project is developed for educational and academic purposes.
