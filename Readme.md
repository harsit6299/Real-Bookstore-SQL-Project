# 📚 Real Bookstore SQL Project

> 📈 A hands-on SQL project simulating database operations for a real-world bookstore — covering everything from basic retrievals to advanced analytics.

---

## 👨‍💻 Developed by: **Harshit Kumar**

🎓 Final-Year Undergraduate | 🎯 Data Enthusiast | 💻 SQL • Python • Power BI  
📍 NIT Patna | 📬 harshitk.ug22.ec@nitp.ac.in  
🔗 [LinkedIn](https://www.linkedin.com/in/harshit-kumar-32bbb7271) 

---

## 🧩 Project Overview

This project involves working with a **relational database** designed for a fictional but realistic bookstore. It includes **three main tables**:

- `📘 Books`
- `🧾 Orders`
- `👤 Customers`

The goal is to extract meaningful insights and reports using **SQL queries** ranging from basic to advanced operations.

---

## 🛠️ Technologies Used

- 🐬 **MySQL / SQL Server / PostgreSQL** (RDBMS)
- 📄 **SQL** (Structured Query Language)
- 📚 **Concepts**: Joins, Aggregations, Filtering, Grouping, Subqueries, and Set Operations

---

## 📂 Database Schema

### 📘 `Books`
| Column           | Type     |
|------------------|----------|
| `book_id`        | INT      |
| `title`          | TEXT     |
| `author`         | TEXT     |
| `genre`          | TEXT     |
| `price`          | DECIMAL  |
| `stock`          | INT      |
| `published_year` | INT      |

### 👤 `Customers`
| Column         | Type     |
|----------------|----------|
| `customer_id`  | INT      |
| `name`         | TEXT     |
| `email`        | TEXT     |
| `country`      | TEXT     |
| `city`         | TEXT     |

### 🧾 `Orders`
| Column         | Type     |
|----------------|----------|
| `order_id`     | INT      |
| `book_id`      | INT      |
| `customer_id`  | INT      |
| `order_date`   | DATE     |
| `quantity`     | INT      |
| `total_amount` | DECIMAL  |

---

## 🔍 Basic SQL Queries

✅ Retrieve all fiction books  
✅ List books published after 1950  
✅ Show Canadian customers  
✅ Get orders placed in November 2023  
✅ Find most expensive book  
✅ Identify low stock items  
✅ Calculate total revenue  
✅ Find customers with large orders  
✅ Display unique genres

---

## 🧠 Advanced SQL Queries

### 🔄 Joins & Aggregations
- 🏆 Most frequently ordered book
- 💵 Top spending customers
- 📦 Total books sold by author
- 🏙️ Cities of customers who spent over $30
- 📊 Total books sold per genre
- 📚 Remaining stock per book (with COALESCE)

### 📌 Example Highlight:

```sql
-- Top 3 Most Expensive Fantasy Books
SELECT * FROM books
WHERE genre = 'Fantasy'
ORDER BY price DESC
LIMIT 3;
