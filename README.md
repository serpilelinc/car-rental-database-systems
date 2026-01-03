# Car Rental Database System

This repository contains a **Car Rental Management System** developed as part of the **Database Systems** course.
The project is a Java desktop application connected to a **Microsoft SQL Server** database and demonstrates relational database design, SQL usage, and Java–database integration using JDBC.

---

## 📌 Project Purpose

The aim of this project is to design and implement a database-driven system that manages:

* Users
* Vehicles
* Rentals
* Payments

The main focus of the project is on **database design**, **SQL Server usage**, and **JDBC-based data access**, rather than advanced UI complexity.

---

## 🛠 Technologies Used

* Java (Swing)
* Maven
* Microsoft SQL Server
* JDBC (SQL Server Driver)
* Draw.io (ER Diagram)

---

## 📁 Project Structure

```
car-rental-database-system/
│
├── src/
│   └── com/
│       └── carrental/
│           ├── dao/        # Database access objects
│           ├── entity/     # Entity classes
│           ├── ui/         # Swing user interface
│           └── util/       # Database connection utilities
│
├── SQLQuery1.sql                 # SQL Server database script
├── Car Rental ER Diagram.drawio.svg
├── DbProject_document.pdf        # Detailed project report
├── pom.xml
└── README.md
```

---

## 🚀 How to Run the Project (Step by Step)

Follow the steps below to run the project on your local machine.

### 1️⃣ Prerequisites

Make sure the following are installed on your system:

* **Java JDK 8 or higher**
* **Microsoft SQL Server**
* **SQL Server Management Studio (SSMS)**
* An IDE such as **IntelliJ IDEA** or **Eclipse**

---

### 2️⃣ Create the Database

1. Open **SQL Server Management Studio (SSMS)**
2. Create a new database named:

   ```
   CarRentalTrackingDB
   ```
3. Open and execute the SQL script included in the repository:

   ```
   SQLQuery1.sql
   ```

This script will create all required tables and database structures.

---

### 3️⃣ Configure Database Connection

Open the following file:

```
src/com/carrental/util/DatabaseConnection.java
```

The project uses the following **SQL Server JDBC configuration**:

```
jdbc:sqlserver://localhost:1433;databaseName=CarRentalTrackingDB;encrypt=false;trustServerCertificate=true
```

Database credentials used in the project:

```
Username: sa
Password: yusuf1905
```

The SQL Server JDBC driver class:

```
com.microsoft.sqlserver.jdbc.SQLServerDriver
```

---

### 4️⃣ Open the Project in an IDE

1. Open **IntelliJ IDEA** or **Eclipse**
2. Select **Open Project**
3. Choose the project root directory
4. Wait for Maven to download all required dependencies

---

### 5️⃣ Run the Application

1. Navigate to the `ui` package
2. Run the main application class
3. The **Car Rental System** user interface will start

---

## 📄 Documentation

A detailed explanation of the database design, ER diagram, and system implementation is available in:

* `DbProject_document.pdf`

---

## 👥 Team Members

* Serpil Elinç
* Sara Ibrahim
* Esmanur Oruç
* Yusuf Elbiz

---

## 📌 Notes

This project was developed for educational purposes as part of a university **Database Systems** course.
