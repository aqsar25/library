## Library Management System Project


**Description:** This project is a Library Management System designed to help users manage the library's resources and operations. It allows users to perform various tasks including:

* **User Management:**
    * Register and manage user accounts
    * View a list of all users
* **Book Management:**
    * Add new books to the database
    * Search for specific books
    * View a list of all books
    * Issue and return books
    * View current user's issued book details
* **Additional Features:**
    * Displays current date and time
    * User-friendly menu for easy navigation

**Technology Stack:**

* Programming Language: C++
* Database: MySQL
* Operating System: Windows

**Instructions:**

1. Install the required software:
    * C++ compiler
    * MySQL
    * Xampp (optional, for easy MySQL management)
2. Download the project source code.
3. Open the project in your preferred C++ IDE.
4. Configure the database connection details in the code. (Refer to the "Example Database Script" section below)
5. Build and run the program.
6. Follow the on-screen instructions to use the system.

**Example Database Script:**

```sql
CREATE DATABASE IF NOT EXISTS library1;

USE library1;

CREATE TABLE users (
  username VARCHAR(30) NOT NULL PRIMARY KEY,
  password VARCHAR(30) NOT NULL
);

CREATE TABLE book (
  BookNo INT NOT NULL PRIMARY KEY,
  Book_Name VARCHAR(30) NOT NULL,
  Author VARCHAR(30) NOT NULL,
  Issued_By VARCHAR(30) DEFAULT 'None'
);

-- Insert sample data
INSERT INTO users (username, password) VALUES ('admin', 'admin');
INSERT INTO book (BookNo, Book_Name, Author) VALUES (1, 'The Lord of the Rings', 'J. R. R. Tolkien');
INSERT INTO book (BookNo, Book_Name, Author) VALUES (2, 'Harry Potter and the Philosopher\'s Stone', 'J. K. Rowling');
```
## Output

![Screenshot 1](https://github.com/aqsar25/library/assets/113085210/30b23098-d3f8-4e66-9ed0-179eaf51fa71)
![Screenshot 2](https://github.com/aqsar25/library/assets/113085210/d3786222-df5c-42cf-963a-de482b0a5b82)
![Screenshot 3](https://github.com/aqsar25/library/assets/113085210/0db30754-5cab-4f0a-b3b3-82d512dc976a)
![Screenshot 4](https://github.com/aqsar25/library/assets/113085210/ded034d3-9a1b-48df-a924-075afe0d3191)
