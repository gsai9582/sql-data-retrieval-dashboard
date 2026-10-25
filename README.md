# SQL Data Retrieval & Sorting Dashboard

An interactive full-stack database application designed for student records retrieval, filtering, departmental grouping, and dynamic column-based sorting.

## 🚀 Features

- **Multi-criteria Sorting:** Sort records dynamically by student name or registration date.
- **Departmental Filtering:** Real-time filtering by academic departments.
- **Aggregated Analytics:** Live query counting total students enrolled per department.
- **Lightweight Architecture:** Powered by Vanilla HTML5/CSS3 frontend and a PHP/MySQL backend.

## 🛠️ Tech Stack

- **Frontend:** HTML5, CSS3
- **Backend:** PHP 8+
- **Database:** MySQL / MariaDB (relational schema with primary keys and indexed foreign keys)

## 📦 Database Schema (`database.sql`)

```sql
CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    department VARCHAR(50) NOT NULL,
    date_joined DATE NOT NULL
);
```

## 💻 Setup & Installation

1. Clone or download this repository into your web server's root directory (e.g., `htdocs` for XAMPP / WAMP):
   ```bash
   git clone https://github.com/gsai9582/sql-data-retrieval-dashboard.git
   ```
2. Start Apache and MySQL via your local server control panel.
3. Import `database.sql` using phpMyAdmin or the MySQL CLI:
   ```bash
   mysql -u root -p < database.sql
   ```
4. Access the application in your browser:
   ```
   http://localhost/sql-data-retrieval-dashboard/index.php
   ```

## 📄 License
MIT License.
