### **Assignment 1:**



### **Problem 1: Student Performance Analytics System:**



### **Part A – Functional Design (Modular Programming)**



* calculate\_average(scores) → Calculates average marks of a student.
* determine\_grade(average) → Assigns a grade based on average.
* top\_student(students) → Returns the student with the highest average.
* passed\_students(students) → Returns a list of students who passed all subjects (each score ≥ 50).



### **Part B – Object-Oriented Design**



* **Class:** StudentAnalytics
* **Attribute:** students\_data → List of student dictionaries.
* **Methods:**
* compute\_results() → Adds average and grade for each student.
* get\_top\_student() → Returns the top student.
* get\_class\_average() → Calculates class average.
* get\_unique\_grades() → Returns set of distinct grades.
* generate\_report() → Returns a summary dictionary with class average, top student, and grade distribution.
* improving\_students() → Returns students whose scores are strictly increasing.
* to\_table() → Converts data to a table-like structure with IDs, names, averages, and grades.





### **Problem 2: Course Enrollment \& Performance System**



### **Part A – Functional Requirements**



* students\_in\_multiple\_courses(courses) → Returns students enrolled in more than one course.
* courses\_with\_many\_students(courses) → Returns courses with more than 2 students.
* student\_course\_mapping(courses) → Maps each student to the number of courses they are enrolled in.
* all\_unique\_students(courses) → Returns a set of all unique students across all courses.



### **Part B – OOP Design**



* **Class**: CourseAnalytics
* **Attribute:** courses\_data → Dictionary of courses.
* **Methods:**
* get\_multi\_course\_students() → Returns students in multiple courses.
* get\_student\_course\_count() → Returns {student: number\_of\_courses}.
* get\_largest\_course() → Returns course with most students.
* generate\_course\_report() → Returns summary dictionary with total courses, total unique students, largest course, and student-course distribution.
* student\_centered\_view() → Converts course-based data to student-centered data: {student: \[list of courses]}.



### **Explanation of Data Structures and Design Choices**



1. #### **Why sets are used for enrollment**



* Used in Problem 2 to store course students, e.g., {"S01", "S02"}.
* Sets automatically prevent duplicate entries.
* Membership checks are fast.
* Ideal for unique student IDs per course.



#### **2.Why tuples are used for fixed scores**



* Used in Problem 1 to store marks, e.g., (78, 85, 90).
* Tuples are immutable, so scores cannot change accidentally.
* Suitable for fixed-length data like subject marks.
* Easy to compute average, max, or min.



#### **3. Why dictionaries are suitable for structured mapping**



* Used in both problems to store structured data:
* Students: {"id":"S01", "name":"Ali", "scores":(78,85,90)}
* Courses: {"Python":{"instructor":"Dr. A", "students":{...}}}
* Key-value mapping allows easy access and update.
* Flexible for adding new fields like average or grade**.**



#### **4.Why classes improve system organization**



* Classes group data (attributes) and operations (methods) together.
* Make code modular, reusable, and easy to read.
* **Example:** StudentAnalytics handles all student-related calculations.
* **Example:** CourseAnalytics handles all course-related analytics.
* Reduces global variables and keeps functions organized.
