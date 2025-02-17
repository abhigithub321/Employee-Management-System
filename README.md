# Employee-Management-System

![Employee Management System](icons/front.gif)

The Employee Management System is a Java-based desktop application designed to manage employee records efficiently. It provides functionalities such as adding, viewing, updating, and deleting employee details. The application uses a MySQL database to store employee information and features a user-friendly graphical interface built using Java Swing.

## Features
- **Splash Screen**: A splash screen is displayed on startup.
- **Login System**: A login page with user authentication.
- **Main Menu**: After successful login, the main menu provides access to different actions.
  - **Add Employee**: Add new employee details.
  - **View Employee**: View employee details.
  - **Remove Employee**: Delete employee records from the database.
  - **Update Employee**: Update existing employee details.
  - **Database**: The system uses MySQL for data storage, and the employee table holds employee details.

## Technologies Used

- **Java**: Core programming language used for developing the application.
- **Java Swing**: Used for creating the graphical user interface (GUI).
- **MySQL**: Database management system used for storing employee records.
- **JDBC**: Java Database Connectivity API used for connecting the Java application with the MySQL database.

## Prerequisites

Before running the application, ensure you have the following installed on your system:

- **Java Development Kit (JDK)**: Version 8 or higher.
- **MySQL Server**: To host the database.
- **MySQL Connector/J**: JDBC driver for MySQL.
- **IDE**: Any Java IDE (e.g., IntelliJ IDEA, Eclipse) for running the project.

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/employee-management-system.git
   cd employee-management-system

2.Database Setup:

-Create a new MySQL database named employeemanagement.
-Run the following SQL script to create the necessary tables:

CREATE TABLE employee (
    empId VARCHAR(20) PRIMARY KEY,
    name VARCHAR(50),
    fname VARCHAR(50),
    dob VARCHAR(20),
    salary VARCHAR(20),
    address VARCHAR(100),
    phone VARCHAR(15),
    email VARCHAR(50),
    education VARCHAR(50),
    addhar VARCHAR(20),
    designation VARCHAR(50)
);

CREATE TABLE login (
    username VARCHAR(50) PRIMARY KEY,
    password VARCHAR(50)
);

INSERT INTO login (username, password) VALUES ('admin', 'admin123');

3.Configure Database Connection:

-Open the conn.java file located in the employee.management.system package.
-Update the database connection URL, username, and password as per your MySQL configuration:

connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/employeemanagement", "root", "yourpassword");

4.Run the Application:

-Open the project in your preferred Java IDE.
-Run the Splash.java file to start the application.

Usage:

1.Login
-Use the default username admin and password admin123 to log in.

2.Main Menu
-Add Employee: Navigate to the "Add Employee" section to enter new employee details.
-View Employee: View the list of all employees in the database.
-Update Employee: Select an employee and update their details.
-Remove Employee: Select an employee and delete their record.

Screenshots
Splash Screen

Login Screen

Main Menu

Add Employee

View Employee

Update Employee

Contributing
Contributions are welcome! If you'd like to contribute, please fork the repository and create a pull request. You can also open an issue to report bugs or suggest new features.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Thanks to all the open-source contributors whose libraries and tools were used in this project.

Special thanks to the Java and MySQL communities for their extensive documentation and support.

Contact
For any queries or feedback, please reach out to abhinavvaidya510@example.com
