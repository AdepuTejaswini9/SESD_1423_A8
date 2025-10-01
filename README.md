**Student Grading System (OOP + Unit Testing)**
**1.Project Overview**
This project implements a Student Grading System using Object-Oriented Programming (OOP) concepts in Python and validates functionality with Unit Testing.
It simulates how a university might manage courses, assign grades, and calculate student GPA.
**2.Features**
Student Management: Each student has a name, ID, and enrolled courses.

Course Representation: Each course has a code, name, and credit value.

Grade Assignment: Students can receive grades (A, B, C, D, F) in courses.

GPA Calculation: GPA is calculated using credit-weighted grade points.

Transcript Generation: Generates a formatted transcript for each student.

Error Handling: Rejects invalid grades.
**3.Technologies Used**
Python 3

Jupyter Notebook

OOP Concepts (Encapsulation, Abstraction, Polymorphism)

Unit Testing (unittest and pytest)
**4.Project Structure**
StudentGradingSystemProject/
│── Student_Grading_System.ipynb   # Main notebook with OOP code + unit tests
│── requirements.txt               # Dependencies file
│── README.md                      # Project documentation

**5.Installation & Running**

1. Clone / Download the Project

Place all files (.ipynb, requirements.txt, README.md) in one folder.

2. Install Dependencies

Run this command in terminal / Anaconda prompt:

pip install -r requirements.txt

3. Run the Notebook

Open Jupyter Notebook and launch:

jupyter notebook Student_Grading_System.ipynb

4. Run Tests with Pytest

Inside the project folder, run:

pytest -q


or in Jupyter Notebook:

!pytest -q


✅ You should see output like:

3 passed in 0.10s

**6.Unit Tests Covered**

GPA Calculation Accuracy – Ensures GPA is correctly calculated.

Invalid Grade Handling – Ensures invalid grades raise ValueError.

No Courses GPA – Ensures GPA returns 0.0 if a student has no courses.

**7.UML Class Diagram**
+-------------------+        +-------------------+        +-------------------+
|     Student       |        |      Course       |        |       Grade       |
+-------------------+        +-------------------+        +-------------------+
| - name: str       |        | - course_code: str|        | - course: Course  |
| - student_id: str |        | - course_name: str|        | - grade_value: str|
| - courses: list   |        | - credits: int    |        +-------------------+
+-------------------+        +-------------------+        | + get_grade_point()|
| + enroll(grade)   |                                      +-------------------+
| + calculate_gpa() |
| + get_transcript()|
+-------------------+

**Learning Outcomes**

Applied OOP principles in Python.

Practiced Unit Testing with both unittest and pytest.

Learned basics of Test-Driven Development (TDD).

Understood how to structure a small software project with docs and requirements.
