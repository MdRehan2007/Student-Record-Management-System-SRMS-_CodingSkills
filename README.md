# Student-Record-Management-System-SRMS-_CodingSkills
Student Record Management System Description 

Header Files & Constants

Description:
The program starts by importing the required C libraries and defining constants used throughout the system.

stdio.h – Input/Output

stdlib.h – File handling and memory

string.h – String comparison & manipulation

STUDENT_FILE – Stores all student records

CREDENTIAL_FILE – Stores login information

🔑 Login Function

Handles user authentication and role detection.

Prompts for username & password

Reads credentials.txt

Compares credentials

Sets currentUser and currentRole

Returns 1 (success) or 0 (fail)

📋 Add Student Function

Adds a new student record to the system.

Takes roll number, name, marks

Opens file in append mode

Writes record into students.txt

Confirms successful addition

🟦 Two-Column UI Cards (Like Your Pictures)
<table> <tr> <td width="50%">
🖥️ Display Students Function

Shows all stored student records in tabular format.

Opens students.txt

Reads each record

Displays Roll, Name, Marks

Handles empty file case

</td> <td width="50%">
🔍 Search Student Function

Finds a specific student using roll number.

Prompts for roll number

Scans each record

Displays details if found

Prints message if not found

</td> </tr> </table>
<table> <tr> <td width="50%">
✏️ Update Student Function

Modifies existing student information.

Creates temporary file

Copies all records

Updates only matching roll number

Replaces old file with updated copy

</td> <td width="50%">
🗑️ Delete Student Function

Deletes a student permanently.

Asks roll number

Skips matching record while copying

Rewrites remaining data

Replaces original file

</td> </tr> </table>
🧭 Main Function

Controls the entire program flow.

Starts login process

Calls correct menu by role

Performs user-selected operation

Ends when user logs out
