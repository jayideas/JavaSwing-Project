# JavaSwing-Project
A simple Java Swing application implementing Create, Read, Update, and Delete (CRUD) operations with a MySQL database using JDBC.

# Java Swing Project

A Java-based desktop application built using **Swing** for GUI development and **JDBC** for database connectivity. This project demonstrates how to perform CRUD operations with separate modules for user, staff, and admin-level management.

## 📁 Project Structure

swing/
├── src/
│ ├── Delete/ # Code for deleting records
│ ├── GetConnection/ # JDBC connection setup
│ ├── Home/ # Main home/dashboard GUI
│ ├── Insert/ # Insert new records
│ ├── OPeration/ # Interfaces for operations
│ ├── OPerationImp/ # Implementation of operations
│ ├── Show/ # Display data from DB
│ ├── UI/ # User Interface (Login, POJO)
│ └── update/ # Update records
├── bin/ # Compiled class files
├── .classpath, .project, .settings/ # Eclipse configuration
└── README.md

markdown
Copy
Edit

## 🛠 Technologies Used

- **Java (Swing)**
- **JDBC** for database connection
- **MySQL (via XAMPP)**
- **Eclipse IDE**

## ✅ Features

- User Login System
- Add, Update, Delete, Show functionalities
- Modular code with separation of logic and UI
- Reusable operation interfaces and implementations

## 🚀 Getting Started

### 1. Install XAMPP

You need to install **XAMPP** to run the MySQL server locally.

- [Download XAMPP](https://www.apachefriends.org/index.html)
- After installing, open the **XAMPP Control Panel** and start the **MySQL** service.

### 2. Clone the repository

```bash
git clone https://github.com/jayideas/JavaSwing-Project.git
3. Open in Eclipse
File → Open Projects from File System → Select the swing/ folder

4. Configure MySQL Connection
Open GetCon.java

Update the JDBC connection string, username, and password to match your MySQL setup (default is usually root with no password)

java
Copy
Edit
Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/your_database", "root", "");
5. Create the Database
Use phpMyAdmin from XAMPP or MySQL Workbench to create your database.

Import the provided SQL schema (if available).

6. Run the Application
Right-click on Home.java or Login.java → Run As → Java Application
