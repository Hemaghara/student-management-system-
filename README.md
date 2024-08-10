# student-management-system-
This Java program is a basic console-based application that interacts with a MySQL database to perform CRUD (Create, Read, Update, Delete) operations on a student records table. The program uses JDBC (Java Database Connectivity) to connect to the database and execute SQL queries. Here's an overview of the key components:

## 1. Database Connection Setup
- The program starts by loading the MySQL JDBC driver and establishing a connection to the database using the specified URL, username, and password.
- If the connection is successful, it prints a confirmation message.

## 2. Menu Options
- The program continuously runs a loop that displays a menu of options to the user, allowing them to:
  - Add a student's details to the database.
  - Remove a student's record from the database.
  - Display all students' details.
  - Search for a student's details based on their roll number.
  - Exit the application.

## 3. Adding a Student
- The `Add_Student_Detail` method prompts the user for student details (roll number, name, address, grade) and inserts the data into the database using a `PreparedStatement`.

## 4. Removing a Student
- The `Remove_Student` method deletes a student's record based on the roll number provided by the user. It uses a `PreparedStatement` to execute the SQL DELETE query.

## 5. Displaying All Students
- The `Display_all_student` method retrieves and displays all records from the student table. It uses a `Statement` object to execute a SELECT query and iterates through the result set to print each student's details.

## 6. Searching for a Student
- The `Search_Student_Detail` method allows the user to search for a student by roll number. It executes a SELECT query using a `PreparedStatement` and displays the student's details if found.

## 7. Exiting the Application
- The `Exit` method is a placeholder that currently just prints a goodbye message. The method also indicates where you would typically close the database connection and clean up resources.

## Key Concepts Covered
- **JDBC Basics:** Establishing a connection, executing SQL queries, and handling exceptions.
- **SQL Operations:** Inserting, deleting, selecting records in a database.
- **User Interaction:** Accepting input from the user and providing corresponding feedback.
- **Error Handling:** Basic exception handling to manage potential issues during database operations.

This program provides a foundation for understanding how Java applications can interact with databases, making it a useful starting point for learning more advanced database programming and Java application development.
