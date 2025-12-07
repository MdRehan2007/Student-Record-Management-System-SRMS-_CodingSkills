# Student-Record-Management-System-SRMS-_CodingSkills
Student Record Management System Description 

<style> /* Github ignores actual CSS, but boxes still look modern via HTML + markdown layout */ </style> <br>
🚀 Code Explanation – Module Overview
<table> <tr> <td width="50%"> <h3>📁 Header Files & Constants</h3> <div> ✔️ `stdio.h` – Input/Output operations ✔️ `stdlib.h` – Memory, process control ✔️ `string.h` – String operations

Constants Used:

STUDENT_FILE → Path to student data

CREDENTIAL_FILE → Path to login data

</div> </td> <td width="50%"> <h3>🔐 Login Function</h3> <div> ✔️ Reads username & password ✔️ Opens `credentials.txt` ✔️ Matches input with stored data ✔️ Sets `currentUser` & `currentRole` ✔️ Returns **1** (success) or **0** (fail) </div> </td> </tr> </table>
<table> <tr> <td width="50%"> <h3>➕ Add Student Function</h3> <div> - Reads **Roll, Name, Marks** - Appends to `students.txt` - Saves in structured format - Prints confirmation message </div> </td> <td width="50%"> <h3>📋 Display Students Function</h3> <div> - Opens students file - Prints table view - Displays roll, name, marks - Handles empty file case </div> </td> </tr> </table>
<table> <tr> <td width="50%"> <h3>🔍 Search Student Function</h3> <div> - Prompts for roll number - Searches each entry - Shows result if match found - Otherwise displays “Not Found” </div> </td> <td width="50%"> <h3>✏️ Update Student Function</h3> <div> - Creates `temp.txt` - Copies all records - Updates matched record - Replaces original file </div> </td> </tr> </table>
<table> <tr> <td width="50%"> <h3>🗑️ Delete Student Function</h3> <div> - Asks for roll to delete - Skips matched record - Writes all others to `temp.txt` - Replaces `students.txt` </div> </td> <td width="50%"> <h3>🧠 Main Function</h3> <div> - Calls login system - Displays correct role menu - Runs until user logs out - Ends program safely </div> </td> </tr> </table>
