# TrackHive
**TrackHive** is a comprehensive Student Attendance and Subject Management System designed to streamline attendance tracking, subject management, and data organization for educational institutions.
It allows administrators and faculty to register students, view attendance data, update, and delete student information. The system is built using Spring Boot, Hibernate, and MySQL for efficient database management and scalability.
# Features
**Student Registration:** Add new students with details like name, student ID, course, and contact information.
**View Attendance:** View attendance records based on various filters such as subject, date, and student.
**Update Student Info:** Update student details like name, course, and contact information.
**Delete Student:** Delete student information based on student ID.
**Subject Management:** Manage subjects, assign faculty, and link students to courses.
**Database Integration:** The system uses MySQL to store and retrieve student and attendance data.

# Tech Stack:
**Java:** The main programming language used for the backend.
**Spring Boot:** Framework for building the REST API.
**Hibernate:** For ORM-based database interactions.
**MySQL:** Database for storing student and attendance information.
**Maven:** For managing project dependencies.
**Postman:** Used for API testing and validation.
**Eclipse:** Integrated development environment (IDE) for development.

# Project :

**TrackHive/
├── src/
│   ├── com/
│   │   ├── controller/
│   │   │   └── StudentController.java
│   │   │   └── AttendanceController.java
│   │   │   └── SubjectController.java
│   │   ├── dao/
│   │   │   └── StudentDAO.java
│   │   │   └── AttendanceDAO.java
│   │   │   └── SubjectDAO.java
│   │   ├── entity/
│   │   │   └── Student.java
│   │   │   └── Attendance.java
│   │   │   └── Subject.java
│   │   ├── service/
│   │   │   └── StudentService.java
│   │   │   └── AttendanceService.java
│   │   │   └── SubjectService.java
│   │   └── utility/
│   │       └── DatabaseConnection.java
├── pom.xml
├── README.md**

# Project :
**com.controller:** Contains the controller classes responsible for handling student, attendance, and subject-related API operations.
**com.entity:** Represents the entities Student, Attendance, and Subject mapped to the database.
**com.dao:** Contains data access objects for performing CRUD operations with the database.
**com.service:** Contains business logic for interacting with the DAO layer and processing data.
**com.utility:** Includes utility classes for managing database connections and other helper functions.

# Database and Table Structure
** The TrackHive project uses a MySQL database to store and manage the following entities: **

**1. Students Table**
Stores information about the students.

student_id (Primary Key):Unique identifier for each student.
name: Name of the student.
course: The course or subject the student is enrolled in.
contact_info: Contact information for the student.
**2. Subjects Table**
Stores information about the subjects.

subject_id (Primary Key): Unique identifier for each subject.
subject_name: Name of the subject.
faculty_id: Foreign Key linking to the Faculty table.
**3. Attendance Table**
Tracks the attendance records for students.

attendance_id (Primary Key): Unique identifier for each attendance record.
student_id: Foreign Key linking to the Students table.
subject_id: Foreign Key linking to the Subjects table.
date: The date of the attendance entry.
status: The attendance status (e.g., present, absent).
**4. Faculty Table**
Stores information about faculty members.

faculty_id (Primary Key): Unique identifier for each faculty member.
name: Name of the faculty member.
contact_info: Contact information for the faculty member.**

This project offers an organized and efficient approach to managing student attendance, subjects, and academic records, ensuring smooth operations and scalability for educational institutions.
For any questions or feedback, feel free to reach out to **bondreashwini648@gmail.com.**






