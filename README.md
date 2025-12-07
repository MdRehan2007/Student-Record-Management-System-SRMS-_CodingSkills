# Student-Record-Management-System-SRMS-_CodingSkills
Student Record Management System Description 


1. Header Files & Global Setup

This section includes the basic libraries required for input/output, memory handling, and string operations.
It also defines two important constants:

STUDENT_FILE → File where all student records are stored

CREDENTIAL_FILE → File containing usernames, passwords, and roles

These definitions make the file handling easier and keep the code organized.

🔹 2. Login System

The login system is the first part executed.
It performs:

Reading username and password from the user

Opening credentials.txt

Comparing the input with stored credentials

Setting the current role (ADMIN, USER, STAFF, GUEST)

If the login matches → system allows access
If not → “Access Denied”

This ensures basic security and restricted access.

🔹 3. Role-Based Menus

Once login is successful, the program redirects the user to the correct menu:

✔ ADMIN

Full access: Add, Display, Search, Update, Delete

✔ STAFF

Can only Display and Search

✔ USER

Can Display and Search

✔ GUEST

Can only Display

Each menu is shown in a loop until the user logs out.

🔹 4. Add Student

This function:

Asks Roll No, Name, Marks

Opens file in append mode

Writes the new student record

Confirms successful addition

It updates the student database without affecting old records.

🔹 5. Display Students

Displays all student records in a clean table-like format.
It:

Opens students.txt

Reads each record

Prints Roll, Name, Marks

Shows a message if file is empty

This is mainly used by Admin, User, Staff, and Guest.

🔹 6. Search Student

This function:

Asks for roll number

Searches file line by line

If found → prints name & marks

If not → shows “Not Found”

Used often by users who want quick lookup.

🔹 7. Update Student

To update a record:

Reads all records one by one

Copies them into a temporary file

Replaces the matching record with new data

Deletes old file

Renames new file

This ensures safe updating without corruption.

🔹 8. Delete Student

Very similar to update, but instead of modifying, it skips the record matching the roll number.
Finally creates a fresh file without the deleted data.

Admin-only feature.

🔹 9. Main Function

This is the control center:

Starts login

Shows correct menu

Performs operations according to role

Ends when user logs out

This keeps the full program flow controlled and stable
