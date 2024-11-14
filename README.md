# Student Record Management System

## Table of Contents
- Overview
- Features
  - Roles and Functionalities
- Modules
- Getting Started
  - Prerequisites
  - Installation
  - Usage
- File Structure
- System Flow
- Project Details
- Contributing
- License

## Overview

The **Student Record Management System** is a C++ console-based application designed to manage and organize student information, staff profiles, attendance records, grades, and notifications in an academic institution. The system operates with three main user roles—**Admin**, **Staff**, and **Student**—each granted specific permissions and functionalities to ensure secure and efficient management of academic records.

This application uses file-based storage for data persistence, allowing for robust and secure record management and retrieval for different users.

## Features

### Roles and Functionalities

This system includes three user roles, each with its own set of permissions:

1. **Administrator**
   - **Student Management**: Add new students, update records, view profiles, and delete student information.
   - **Staff Management**: Add and remove staff profiles, assign subjects, and manage contact information.
   - **Attendance Management**: Record student attendance, update records as needed, and generate attendance reports.
   - **Grades and Exams**: Input and view student grades, create exam schedules, and set up timetables.
   - **Notifications and Complaints**: Post notifications for users and view student complaints.

2. **Staff**
   - **Profile Management**: View and update personal staff profile details.
   - **Student Record Management**: Add or update student attendance and grades for the assigned subjects.
   - **Reports**: Generate reports on attendance and grades for students in their subject areas.

3. **Student**
   - **Profile Access**: View personal information, including admission number, email, and department.
   - **Attendance and Grades**: Check attendance status and view grades for enrolled subjects.
   - **Notifications**: Access announcements or updates posted by the admin.
   - **Complaints**: Submit complaints or feedback to the admin.

## Modules

### Core Modules

- **Student Module**: Manages all student-related operations, including admission, attendance, and grade tracking.
- **Staff Module**: Allows staff members to manage their assigned subjects, such as updating attendance and grades.
- **Admin Module**: Provides administrators with full control over the system, including user management and complaint handling.
  
### Utility Modules
- **File Handling**: Implements binary files to securely store and quickly retrieve data.
- **Date and Time Utilities**: Used to record the dates for attendance and notifications.

## Getting Started

### Prerequisites

- **C++ Compiler**: A compatible C++ compiler (such as GCC or MinGW for Windows).
- **Windows OS**: This application is designed specifically for Windows, as it uses Windows-specific commands.

### Installation

1. **Clone this repository** to your local machine.
2. **Navigate to the project directory** in the terminal.
3. **Compile the project** using your C++ compiler.

### Usage

1. **Run the compiled executable file** to start the application.
2. Upon launch, select the login type: **Admin**, **Staff**, or **Student**.
3. Depending on the login type, users will see different options:
   - **Admin**: Manage student and staff records, view attendance and grades, handle notifications, and address complaints.
   - **Staff**: View and manage attendance and grades for their assigned students.
   - **Student**: View their profile, attendance, and grades, and submit complaints if necessary.
4. **Log out** after completing tasks to return to the main login screen.

## File Structure

- **student.dat** - Stores student data, including grades, attendance, and profile details.
- **staff.dat** - Contains information about staff members, including staff ID, assigned subjects, and email.
- **notification.dat** - Stores notifications posted by the admin for all users.
- **table.dat** - Contains the exam schedule, including subjects, dates, and start/end times.
- **complaint.dat** - Stores complaints submitted by students for admin review.

## System Flow

1. **Initial Setup**: When run for the first time, the application checks for the necessary data files and initializes them if they do not exist.
2. **Login and Authentication**: Users select their role (Admin, Staff, Student) and authenticate using predefined credentials.
   - **Admin Password**: "OOP" by default.
   - **Staff and Student Passwords**: Use the assigned USN or staff ID as the default password.
3. **Role-Based Access**: Each user role has access to a customized menu, specific to their permissions.
4. **Data Persistence**: All data is stored in binary files, ensuring data consistency and security across sessions.

## Project Details

This project demonstrates several important C++ programming concepts:

- **Classes and Inheritance**: Defines separate classes for Admin, Staff, and Student roles, each with specific methods and attributes.
- **File Handling**: Uses binary files to securely store data for each role, ensuring persistence.
- **Operator Overloading**: Overloads operators to simplify attendance management tasks.
- **Inline Functions**: Utilizes inline functions for quick screen clearing (`clrscr`) and title display.
- **Macros and Constants**: Defines constants like `F_NOT_FOUND`, `USN_NOT_FOUND`, and `SUCCESS` for consistent function returns.

## Contributing

Contributions to this project are welcome. If you would like to contribute:

1. Fork this repository.
2. Create a new branch for your feature or fix.
3. Submit a pull request with a clear description of your changes.

Please ensure your code is well-documented and follows the project’s coding conventions.


---

