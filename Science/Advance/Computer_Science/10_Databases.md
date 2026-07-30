---
tags:
  - computer-science
  - advance
  - databases
  - sql
  - ipst
source: "IPST (สสวท.) Computer Science Curriculum B.E. 2551 (2008, revised 2560/2017)"
created: 2026-07-30
course_codes: ["ว333"]
---

# Databases — ฐานข้อมูล

> *"Data is the new oil. It's valuable, but if unrefined it cannot really be used."* — Clive Humby (2006)

A database (ฐานข้อมูล) is an organized collection of data stored so it can be accessed, managed, and updated efficiently. Where a spreadsheet works for a few thousand rows, a database scales to millions, supports concurrent users, enforces data integrity, and offers a powerful query language: **SQL**. Almost every modern application — banking, e-commerce, social media, school records — depends on a database behind the scenes.

This note covers the relational model (ตาราง, แถว, คอลัมน์), keys (primary/foreign), ER diagrams, the core SQL operations (CRUD: SELECT, INSERT, UPDATE, DELETE), filtering with WHERE, JOINs, an introduction to normalization, NoSQL, and principles of good database design.

---

## 1 | Course Coverage

### ม.6 (ว333)

| Semester | Scope | Key Skills |
|---|---|---|
| **Semester 1** | Relational model, tables, keys, ER diagrams, basic SQL | Write SELECT/INSERT/UPDATE/DELETE, design a schema |
| **Semester 2** | JOINs, normalization, NoSQL overview, design principles | Normalize to 3NF, choose SQL vs NoSQL |

---

## 2 | Key Terminology

| Thai | English | Symbol/Notes |
|---|---|---|
| ฐานข้อมูล | Database | Organized data store |
| ระบบจัดการฐานข้อมูล | DBMS | MySQL, PostgreSQL, SQLite |
| ตาราง | Table / Relation | Rows × columns |
| แถว / ระเบียน | Row / Record | One entity instance |
| คอลัมน์ / ฟิลด์ | Column / Field | One attribute |
| คีย์หลัก | Primary Key (PK) | Unique, non-null identifier |
| คีย์นอก | Foreign Key (FK) | References PK in another table |
| แบบจำลองเชิงสัมพันธ์ | Relational model | Tables + relationships |
| แผนภาพ ER | ER Diagram | Entity-Relationship diagram |
| การทำให้เป็นปกติ | Normalization | Remove redundancy |
| คิวรี่ | Query | Data request (SQL) |
| ฐานข้อมูล NoSQL | NoSQL database | Document/key-value/graph |

---

## 3 | Key Concepts

### 3.1 The Relational Model (แบบจำลองเชิงสัมพันธ์)

A **relational database** (ฐานข้อมูลเชิงสัมพันธ์) organizes data into **tables** (ตาราง). Each table has:

- **Columns / fields** (คอลัมน์) — the attributes, e.g. `student_id`, `name`, `gpa`.
- **Rows / records** (แถว / ระเบียน) — one entity instance, e.g. one student.

Example table `students`:

| student_id (PK) | name | gpa | class_id (FK) |
|---|---|---|---|
| 1 | Somchai | 3.5 | 101 |
| 2 | Nicha | 3.8 | 102 |
| 3 | Akira | 2.9 | 101 |

### 3.2 Keys (คีย์)

- **Primary Key (PK)** (คีย์หลัก) — uniquely identifies each row; must be unique and not null. Example: `student_id`.
- **Foreign Key (FK)** (คีย์นอก) — a column referencing the PK of another table, creating a relationship.
- **Composite key** — a PK made of two or more columns combined.

```
students.class_id  ──FK──>  classes.class_id (PK)
```

### 3.3 ER Diagrams (แผนภาพ ER)

An **Entity-Relationship diagram** (แผนภาพ ER) visualizes the schema:

- **Entities** (เอนทิตี) → rectangles → become tables.
- **Attributes** (แอตทริบิวต์) → ovals → become columns.
- **Relationships** (ความสัมพันธ์) → diamonds, with **cardinality**:

| Notation | Meaning | Example |
|---|---|---|
| 1 : 1 | One-to-one | Person ↔ Passport |
| 1 : N | One-to-many | Class → Students |
| M : N | Many-to-many | Students ↔ Courses (needs a junction table) |

### 3.4 SQL — The Core Operations (CRUD)

| Operation | SQL keyword | Purpose |
|---|---|---|
| **Create** | `INSERT` | Add a row |
| **Read** | `SELECT` | Query data |
| **Update** | `UPDATE` | Modify existing rows |
| **Delete** | `DELETE` | Remove rows |

```sql
-- Create
INSERT INTO students (student_id, name, gpa, class_id)
VALUES (4, 'Ploy', 3.9, 102);

-- Read
SELECT name, gpa FROM students WHERE gpa >= 3.5;

-- Update
UPDATE students SET gpa = 3.6 WHERE student_id = 3;

-- Delete
DELETE FROM students WHERE student_id = 4;
```

### 3.5 Filtering and Sorting (WHERE, ORDER BY)

```sql
SELECT name, gpa
FROM students
WHERE gpa >= 3.0 AND class_id = 101
ORDER BY gpa DESC;
```

Operators: `=`, `<>`, `>`, `<`, `>=`, `<=`, `BETWEEN`, `IN (...)`, `LIKE '%cha'`, `AND`, `OR`, `NOT`.

Aggregations: `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`, with `GROUP BY` and `HAVING`.

```sql
SELECT class_id, AVG(gpa) AS avg_gpa
FROM students
GROUP BY class_id
HAVING AVG(gpa) > 3.0;
```

### 3.6 JOINs (การเชื่อมตาราง)

A **JOIN** combines rows from two or more tables based on a related column.

```sql
-- INNER JOIN: only matching rows
SELECT s.name, c.class_name
FROM students s
INNER JOIN classes c ON s.class_id = c.class_id;
```

| JOIN type | Returns |
|---|---|
| `INNER JOIN` | Only rows with matches in both tables |
| `LEFT JOIN` | All left rows + matching right (nulls if none) |
| `RIGHT JOIN` | All right rows + matching left |
| `FULL OUTER JOIN` | All rows from both tables |

### 3.7 Normalization (การทำให้เป็นปกติ)

Normalization (การทำให้เป็นปกติ) reduces redundancy and anomalies by splitting tables. The common **normal forms (NF)**:

- **1NF** — atomic values; no repeating groups.
- **2NF** — 1NF + no partial dependency (every non-key column depends on the whole PK).
- **3NF** — 2NF + no transitive dependency (non-key columns depend only on the PK).

Goal: each fact stored **once**, in the right place.

### 3.8 NoSQL Overview (ฐานข้อมูล NoSQL)

**NoSQL** databases relax the relational rules for flexibility and scale:

| Type | Example | Stores |
|---|---|---|
| **Document** | MongoDB | JSON-like documents |
| **Key-value** | Redis | Key → value pairs |
| **Column-family** | Cassandra | Wide columns |
| **Graph** | Neo4j | Nodes + edges |

Use NoSQL for: rapidly changing schemas, massive horizontal scale, hierarchical/nested data. Use SQL (relational) for: structured data, complex queries, strict consistency.

### 3.9 Database Design Principles

1. **Identify entities** and their attributes first.
2. **Choose a clear primary key** for every table (often an auto-increment ID).
3. **Define relationships** with foreign keys.
4. **Normalize** to at least 3NF to avoid redundancy.
5. **Add indexes** on frequently filtered columns for speed.
6. **Enforce constraints**: `NOT NULL`, `UNIQUE`, `CHECK`.

---

## 4 | Common Problem Types

### Type 1: Write a SELECT with WHERE

> Find all students in class 101 with GPA of at least 3.0.

**Solution:**
```sql
SELECT student_id, name, gpa
FROM students
WHERE class_id = 101 AND gpa >= 3.0
ORDER BY gpa DESC;
```

### Type 2: JOIN Two Tables

> List each student's name with their class name.

**Solution:**
```sql
SELECT s.name, c.class_name
FROM students s
INNER JOIN classes c ON s.class_id = c.class_id;
```

### Type 3: Python + SQLite (sqlite3)

> Create a database, insert data, and query it from Python.

**Solution:**
```python
import sqlite3

conn = sqlite3.connect(":memory:")   # in-memory DB
cur = conn.cursor()

cur.execute("""
CREATE TABLE students (
    student_id INTEGER PRIMARY KEY,
    name TEXT,
    gpa REAL
)
""")
cur.executemany("INSERT INTO students VALUES (?, ?, ?)",
    [(1, "Somchai", 3.5), (2, "Nicha", 3.8), (3, "Akira", 2.9)])
conn.commit()

for row in cur.execute("SELECT name, gpa FROM students WHERE gpa >= 3.0 ORDER BY gpa DESC"):
    print(row)
# ('Nicha', 3.8)
# ('Somchai', 3.5)

conn.close()
```

---

## 5 | Cross-Links

- [[07_Data_Structures]] — tables/dicts mirror relational structure
- [[09_Computer_Systems_and_Networks]] — DBMS is server software over networks
- [[11_Artificial_Intelligence]] — ML training data often sourced from databases
- [[../../Fundamental/17_Sets|Mathematics: Sets]] — relational algebra = set operations
