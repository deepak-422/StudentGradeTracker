# StudentGradeTracker

**StudentGradeTracker** is a C++ application that calculates and manages student grades, generates report cards, and stores student data in a MySQL database.

## Features
- **Input**: Takes student marks for multiple subjects (e.g., Subject1, Subject2, Subject3).
- **Processing**: Calculates the average and assigns a grade based on predefined criteria.
- **Database Integration**: Updates the student’s grade and average in a MySQL database.
- **Report Generation**: Generates a student report card with their grades and performance.

## Requirements
- **C++ Compiler**: Any modern C++ compiler (e.g., g++, MSVC).
- **MySQL**: A running instance of MySQL (with a database and a `Student` table).
- **MySQL C++ Connector**: Ensure that the MySQL C++ connector library is set up for the program to interact with the database.

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/deepak-422/StudentGradeTracker.git
Database Setup:

Create a MySQL database (e.g., mydb) and a Student table with columns for RollNo, Name, Avg, and Grade.

Example SQL for creating the table:

sql
Copy
CREATE TABLE Student (
    RollNo VARCHAR(10),
    Name VARCHAR(50),
    Avg FLOAT,
    Grade VARCHAR(5)
);
Compile the C++ Code:

Ensure you have the MySQL C++ connector installed and linked to your project.

Compile the main C++ file (main.cpp):

bash
Copy
g++ main.cpp -o StudentGradeTracker -lmysqlclient
Run the Program:

Execute the program:

bash
Copy
./StudentGradeTracker
How to Use
Input: Enter student details (RollNo, marks for subjects) when prompted.

Output: The program will calculate the average, assign a grade, and update the MySQL database with the results.

Report: After calculating grades, the program will display the report card for the student.

License
This project is licensed under the MIT License.
