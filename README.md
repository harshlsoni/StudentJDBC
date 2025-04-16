
# 🎓 Student Management System (Java + MySQL)

This project is a **Student Management System** built using **Java** and **MySQL**. It allows an admin to manage student records efficiently. The system supports storing, retrieving, updating, and deleting student details based on their PRN (Permanent Registration Number).

## 🛠️ Features

- ✅ Add a new student to the database  
- 🔍 Search for a student using PRN  
- ✏️ Update student details using PRN  
- 🗑️ Delete student records from the database  
- 🗂️ Store student details including:
  - PRN
  - Name
  - Date of Birth
  - Marks

## 💻 Technologies Used

- **Java** (Core Java, JDBC)
- **MySQL** (Relational Database)
- **JDBC (Java Database Connectivity)**

## 🧾 Prerequisites

Before running this project, ensure you have:

- Java (JDK 8 or above)
- MySQL Server
- MySQL JDBC Driver
- An IDE like IntelliJ IDEA or VS Code (with Java extensions)

## 🗃️ Database Setup

1. Create a database in MySQL:

```sql
CREATE DATABASE student_management;
USE student_management;
```

2. Create a table:

```sql
CREATE TABLE students (
    prn VARCHAR(20) PRIMARY KEY,
    name VARCHAR(50),
    dob DATE,
    marks DOUBLE
);
```

3. Update the DB connection URL, username, and password in your Java code:
```java
Connection con = DriverManager.getConnection("jdbc:mysql://localhost:3306/student_management", "root", "your_password");
```

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/student-management-system-java.git
cd student-management-system-java
```

2. Open the project in your preferred Java IDE.

3. Compile and run the main class.

## 📸 Screenshots

![Screenshot 2025-04-16 184816](https://github.com/user-attachments/assets/e08b06c2-5b83-4f57-91cf-83eefce51dd8)

![Screenshot 2025-04-16 184842](https://github.com/user-attachments/assets/d1e35a36-2cad-4509-8639-93bc240137f7)

## 📌 Future Improvements

- Add GUI using JavaFX or Swing  
- Add login system for admin  
- Input validation and error handling  
- Export student data to CSV
