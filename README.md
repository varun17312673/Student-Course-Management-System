# Student-Course-Management-System
A simple SQL project designed to manage students, courses, faculty, and enrollments.
This project includes:

✔ Database schema
✔ Sample data
✔ 25 practical SQL queries (easy → moderate)
✔ Perfect for beginners adding projects to GitHub or resume

📦 Student-Course-Management-System
 ┣ 📄 student_course_management_system.sql
 ┗ 📄 README.md

*Database Relationship Diagram*
 +-----------+         +-----------+        +-------------+
| Students  | 1     ∞ | Enrollments | ∞    1 | Courses     |
+-----------+         +-------------+        +-------------+
| student_id|-------> | student_id  |        | course_id   |
| name      |         | course_id   | <----- | faculty_id  |
| email     |         | enroll_date |        | course_name |
+-----------+         +-------------+        +-------------+
                                                |
                                                ∞
                                                |
                                           +------------+
                                           |  Faculty   |
                                           +------------+
                                           | faculty_id |
                                           | experience |
                                           +------------+
