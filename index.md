
---
layout: default
title: Portfolio
---

# Cybersecurity & Java Portfolio

Welcome! This site showcases compact, working projects that demonstrate API design, incident response skills, and practical automation.

> **Certifications**: Security+ • CySA+ • AWS Cloud Practitioner
> **Focus**: SOC Analyst • IT Audit • Risk/Compliance • Blue Team

---

## 🔹 Project 1 — Apply Filters to SQL Queries


Category: Cybersecurity / Data Analysis



Project Description


This project demonstrates how I applied SQL queries with filters to investigate potential security incidents and update employee systems. I worked with system log and employee data to identify unusual login activity and determine which employee machines required updates.

Key Tasks & Examples


🔹 Investigated After-Hours Failed Logins


Wrote SQL queries to filter failed login attempts that occurred after 18:00. This allowed me to identify suspicious after-hours access patterns.

![IMG_8746](https://github.com/user-attachments/assets/535f7796-d0a5-4faa-a9ca-870ae3ebb7f1)

🔹 Analyzed Logins on Specific Dates


Queried login data for suspicious events that occurred on 2022-05-08 and 2022-05-09. I used logical operators (OR) to filter for multiple dates at once.

[Insert Screenshot: Date-Based Query & Output]

🔹 Detected Foreign Login Attempts


Retrieved all login attempts that occurred outside of Mexico using a NOT LIKE 'MEX%' filter. This helped isolate unusual geographic login activity.

[Insert Screenshot: Outside Mexico Query & Output]

🔹 Identified Employees for Security Updates
Pulled employee machines from the Marketing department (East building).

Retrieved employees in Finance OR Sales departments.

Retrieved employees not in IT to apply specialized updates.



[Insert Screenshot: Employee Queries & Output]

SQL Techniques Used
Filtering with WHERE clauses

Logical operators: AND, OR, NOT

Pattern matching with LIKE and wildcards (%)

Querying across multiple tables: log_in_attempts, employees

Outcome


This project highlights my ability to apply SQL to real-world cybersecurity use cases such as:

Investigating failed login attempts

Detecting abnormal login activity

Supporting IT teams with system updates



It demonstrates both technical SQL query skills and practical security problem-solving.
**How to Run**
```bash
javac ChatPortfolioServer.java
java ChatPortfolioServer
# Server: http://localhost:8080
