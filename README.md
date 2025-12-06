# Student Management System (C Program)

This project is a simple file-based Student Management System written in C.
It supports Admin, Staff, and Guest roles with different access levels.
Users log in using a credentials file, and all student records are stored in a text file.

**📌 Features**
🔐 User Login System

Credentials stored in credentials.txt

Each user has:

Username

Password

Role: admin, staff, or guest

**👤 Role-based Menus**
| Role      | Add | Display | Search | Update | Delete |
| --------- | --- | ------- | ------ | ------ | ------ |
| **Admin** | ✔   | ✔       | ✔      | ✔      | ✔      |
| **Staff** | ✔   | ✔       | ✔      | ✔      | ✖      |
| **Guest** | ✖   | ✔       | ✔      | ✖      | ✖      |

**📁 File Structure**

students.txt
Stores student records in the format:

roll name mark


Example:

101 John 88.50


credentials.txt
Stores login data:

username password role


**Example:**

admin admin123 admin
staff1 staff123 staff
guest1 guest123 guest

**🧑‍💻 Functionalities**
Student Operations

Add Student

Display All Students

Search Student by Roll Number

Update Student Details

Delete Student (Admin-only)

**Menu System**

Separate menus for Admin, Staff, and Guest.

**Automatically selected after login.**

▶️ How to Run
1. Compile
gcc main.c -o sms

2. Create Required Files

Create credentials.txt:

admin admin123 admin
staff1 staff123 staff
guest1 guest123 guest


(Optional) Create an empty students.txt:

(touch students.txt)

3. Run Program
./sms

📘 Example Usage
Login Prompt
USERNAME: admin
PASSWORD: admin123
Logged in as: admin

Admin Menu
ADMIN MENU
1.Add
2.Display
3.Search
4.Update
5.Delete
6.Logout
