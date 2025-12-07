# Student-Record-Management-System-SRMS-_CodingSkills
Student Record Management System Description 

<table> <tr> <td>
📌 Header Files & Constants

The program uses three important C libraries:

stdio.h → Input/Output

stdlib.h → Memory & system functions

string.h → String handling

Constants defined:

STUDENT_FILE → Path to student records

CREDENTIAL_FILE → Path to login credentials

</td> <td>
🔐 Login Function

The login system:

Prompts for username & password

Reads from credentials.txt

Compares input with stored values

Sets currentRole and currentUser

Returns 1 for success, 0 for failure

</td> </tr> <tr> <td>
➕ Add Student Function

This function:

Takes Roll, Name, Marks

Opens students.txt in append mode

Stores the new record

Prints success message

</td> <td>
📋 Display Students Function

This function:

Opens file in read mode

Reads each student record

Prints Roll, Name, Marks in table format

Handles empty file case

</td> </tr> <tr> <td>
🔍 Search Student Function

Searches student by roll number:

Reads each record

Compares roll number

Shows details if found

Displays “Not Found” message if missing

</td> <td>
✏️ Update Student Function

Updates an existing record:

Creates temp.txt

Copies all records

Updates matching student

Replaces old file with updated version

</td> </tr> <tr> <td>
🗑️ Delete Student Function

Deletes a record:

Creates temporary file

Copies all records except the target

Deletes original file

Renames temp.txt to students.txt

</td> <td>
🧠 Main Function

Controls the entire program:

Calls loginSystem()

Redirects user to correct menu

Exits if login fails

</td> </tr> </table>
