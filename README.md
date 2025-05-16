# 📚 Library Management System – Java Swing + XAMPP (MySQL)

👨‍💻 **Developer:** Imtiaz Ahmad Tanvir  
🛠️ **Tech Stack:** Java Swing, JDBC, MySQL (XAMPP), NetBeans/IntelliJ

---

## ✅ Project Overview

This Library Management System is a desktop-based application built with **Java Swing** for the frontend and **MySQL (via XAMPP)** for the backend database. It is designed to streamline and simplify library operations such as book tracking, user registration, borrowing/returning books, and reporting.

---

## 🚀 Features

- 📖 **Add, Update, Delete Books**
- 👥 **Register and Manage Library Users**
- 🔄 **Issue and Return Books**
- 📅 **Due Date & Fine Calculation**
- 📊 **View Issued Book Records**
- 🔍 **Search Functionality (Books/Users)**
- 🔐 **Admin Login Authentication**
- 💾 **MySQL Database Connectivity (JDBC)**

---

## 🖥️ User Interface

- Built using **Java Swing**
- Responsive layout for desktop use
- Organized navigation (Home, Books, Users, Transactions, Reports)

---

## 💾 Database Design (MySQL via XAMPP)

Key Tables:
- `books` – Book ID, Title, Author, Publisher, Quantity
- `users` – User ID, Name, Contact, Role
- `issue_records` – Issue ID, Book ID, User ID, Issue Date, Return Date, Fine

Use **phpMyAdmin** in XAMPP to create the database and run the provided SQL dump.

---

## ⚙️ Installation & Setup

1. Install [XAMPP](https://www.apachefriends.org/index.html) and start Apache & MySQL.
2. Create a new database (e.g., `library_db`) via phpMyAdmin.
3. Import the `library_db.sql` file (provided).
4. Open the Java project in NetBeans/IntelliJ.
5. Update the database connection settings in your Java class:
   ```java
   Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/library_db", "root", "");
