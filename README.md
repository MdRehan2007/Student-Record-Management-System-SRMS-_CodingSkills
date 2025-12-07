# Student-Record-Management-System-SRMS-_CodingSkills
Student Record Management System Description 

📘 Header Files & Constants

This section contains the required libraries and fixed constants used across the project.

#include <stdio.h> — Standard input/output

#include <stdlib.h> — File handling & utilities

#include <string.h> — String comparison & manipulation

📁 STUDENT_FILE — Stores all student information

🔑 CREDENTIAL_FILE — Stores usernames, passwords, and roles
------------------------------------------------------------------------------------------------------------------

🔐 Login Function

This function handles the entire authentication process.

Prompts for username and password

Reads credentials from credentials.txt

Compares user input with stored data

Sets currentUser & currentRole when correct

Returns 1 if success, 0 if login fails

🧭 Main Menu Controller

Directs the user to the correct menu based on role.

Checks the role (ADMIN / STAFF / USER / GUEST)

Loads respective menu

Ensures restricted access for lower roles

👑 Admin Menu

Admin has full privileges in the system.

➕ Add Student

📋 Display Students

🔍 Search Student

✏️ Update Student

🗑️ Delete Student

🚪 Logout

👤 User Menu

User has limited access.

📋 Display Students

🔍 Search Student

🚪 Logout

👨‍🏫 Staff Menu

Similar to User with viewing options.

📋 Display Students

🔍 Search Student

🚪 Logout

👁️ Guest Menu

Guest can only view records.

📋 Display Students

🚪 Logout

➕ Add Student Function

Adds a new student entry to the database.

Takes Roll No, Name, Marks

Appends data to students.txt

Shows “Student added successfully!”

❗ Used only by Admin

📋 Display Students Function

Shows all stored student records.

Opens file in read mode

Prints Roll, Name, Marks for each record

If no file found → prints “No students found”

🔍 Search Student Function

Searches for a student using roll number.

Asks for roll number

Compares with each entry

If matched → Displays Name + Marks

If not → Shows “Student not found”

✏️ Update Student Function

Modifies an existing record safely.

Creates a temporary file

Copies all data

Updates only the matched student

Replaces old file with updated data

🔐 Admin only

🗑️ Delete Student Function

Deletes a student permanently.

Asks for roll number

Skips matching record while copying

Writes all others into a temp file

Replaces original file

🛑 Admin only

🧠 Main Program Flow

Controls the entire execution order.

Login

Show menu based on role

Execute selected operations

Loop until logout

Program ends gracefully

