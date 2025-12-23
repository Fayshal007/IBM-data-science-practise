# Python DB-API Practice

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Database-orange?logo=databricks&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?logo=github&logoColor=white)

---

## 📌 Overview
This repository contains my **practice work on accessing databases using Python DB-API**.  
The goal of this practice is to understand how Python applications interact with relational databases using connections, cursors, and SQL queries.

This practice is part of my learning journey in **Python, SQL, and data handling**, focusing on real-world database operations.

---

## 🛠️ Topics Covered
- Understanding **DB-API concepts**
- Creating a **database connection**
- Using **cursor objects**
- Executing SQL queries
- Fetching query results
- Properly **closing database resources**

---

## 📂 Example Code Practiced
```python
from dbmodule import connect

# Create connection object
connection = connect('databasename', 'username', 'password')

# Create a cursor object
cursor = connection.cursor()

# Execute SQL query
cursor.execute('SELECT * FROM mytable')

# Fetch results
results = cursor.fetchall()

# Free resources
cursor.close()
connection.close()
