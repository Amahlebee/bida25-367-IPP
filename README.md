# bida25-367-IPP
Student grade management system 
The student grade management system is developed to help a school manage its students grades in an organized neat and iffecient way. The program was devided into three sections: section A focused on basic input output and scaler objects, Section B focused on on expanding the program by introducing lists and tuples 
and section C further improved the program using dictionaries to make student information easier to add, update, search and remove.

SECTION A - Scalar Objects And Loops 
In section A the program starts with the basic components of a grading system. The user of the program is asked to enter the number of students in the class.
This number is then stored in a variable using int() because the number of students should be a whole number.
The program then uses a for Loop to repeat the process for every student. For every student the user of the program enters the students names and grades.
The grade is then stored as a float() so that the program can accept both whole numbers and decimals.
The program also includes grade validation to make sure that the numbers inputed are in between 0 and 100. 
A while loop is also used to make sure that the program user is repeatedly asked for a grade until a valid value is entered.
 Once all the grades have been entered into the program, it the calculates the total and average grade.

 SECTION B- Lists And Tuples
 Section B expands the grading system so that the students can have grade for many subjects. The program uses three subjects which are maths, english and and science.
 A list is used to store the grades belonging to each student, This is important because it allows for multiple values to be stored together and can be changed if necessary.
 The program also uses a tuple to represent each student. A tuple can contain the student's name and their list of grades, for example, ("Amahle", [85, 90, 80])
 The program uses loops to go through each student and each subject, allowing the user to enter all the required grades. The append() method is used to add each grade to the student's list. The program then calculates the average for each student using sum(grades) / len(grades).
 Finally, the program displays a summary table containing each student's name, their individual subject grades, and their average.

 SECTION C- Dictionaries 
 Section C changes the way student information is stored by replacing the list of tuples with dictionaries. Dictionaries are useful because information can be stored using a key and a value. In this section, the student's name is used as the key, while another dictionary containing their subjects and grades is used as the value.
 The program begins with an empty dictionary using students = {}. When a new student is entered, their grades are stored in another dictionary and then added to the main dictionary using students[name] = grades.
 The program can also update an existing student's grades by accessing their name and subject This allows a particular grade to be changed without affecting the other grades. A student can also be removed from the system using the del statement, such as del students[name].

 Section D: Functions and Error Handling

Section D improves the organisation and maintainability of the program by dividing repetitive tasks into reusable functions.

The main functions include:

- add_student() which collects a student's name and subject grades and stores the record.
- calculate_average() which calculates the average of a student's grades.
- display_student() which displays an individual student's grades and average.
- display_summary() which displays the records of all students.
- search_update() which searches for a student and allows their grades to be updated.

The program also uses `try` and `except` blocks to handle non-numeric grade inputs. Validation checks ensure that grades are within the permitted range of 0 to 100. The program displays informative messages when a student cannot be found, a subject is invalid, or an incorrect grade is entered.

A menu allows users to select the operation they want to perform

 Section C also allows the user to view all grades for a particular subject across the entire class. The program uses a for loop with .items() to go through each student's name and grades.
 The program also includes a search feature that allows the user to enter a student's name and retrieve their grades and average. The program first checks whether the student exists using if search in students:. If the student is found, their grades are retrieved and their average is calculated
 

Section E

 1. Project Overview

The Student Grade Management System is a Python program that manages student records and grades. Section E introduces Object-Oriented Programming (OOP) by organising the program into classes and methods.

The system allows users to add students, record and update grades, calculate averages, search for and remove students, and sort records by average or subject grades

The program contains two main classes:

Student Class
- Stores the student's name and grades.
- Adds and validates grades.
- Calculates the student's average.
- Displays student details.

Gradebook Class
- Stores and manages Student objects.
- Adds, searches for, and removes students.
- Displays all student records.
- Sorts students by average or subject grade.

The `main()` function provides a menu for users to interact with the system.

4. Features

- Add students and record grades for Math, English, and Science.
- Display individual student records or all students.
- Calculate student averages.
- Search for students by name.
- Update grades and remove students.
- Sort students by average or subject grade.
- Validate grades between 0 and 100.
- Handle duplicate names and invalid inputs.

## 5. Setup Instructions

1. Install Python and open PyCharm.
2. Save the program as `section_e.py`.
3. Run the program in PyCharm or use the terminal:

```bash
python section_e.py
```

## 6. Example Input and Output

```text
Enter your choice: 1
Enter student name: Amahle
Enter Math grade: 80
Enter English grade: 90
Enter Science grade: 70
Student added successfully.
```

Displaying the student's details:

```text
Student: Amahle
Math : 80.0
English : 90.0
Science : 70.0
Average: 80.0
```

7. Testing Summary

| Test case | Expected result |
|---|---|
| Add student | Student record is saved |
| Add duplicate student | Error message displayed |
| Enter invalid grade | Input rejected |
| Search for student | Details displayed if found |
| Update or remove student | Record updated or removed |
| Sort students | Records displayed in descending order |
| Student has no grades | Average is 0 |

Actual test results should be recorded after running the program.

8. Assumptions and Limitations

- Grades must be between 0 and 100.
- Duplicate student names are not allowed, regardless of capitalisation.
- The program manages Math, English, and Science through its menu.
- Student records are stored in memory and are lost when the program closes.
- Sorting uses Python's built-in `sorted()` function.


 Student Grade Management System – Section F

 1. Project Overview

Section F introduces advanced features to the Student Grade Management System. The program allows users to enter student names and grades, calculate averages, search for students, and sort student records.

 2. Technologies Used

- Python
- PyCharm
- Object-Oriented Programming (OOP)
- Bubble sort
- Exception handling

 3. Class Architecture

The program has two main classes:

**Student Class**
- Stores student names and grades.
- Validates grades between 0 and 100.
- Calculates student averages.

**Gradebook Class**
- Adds and stores students.
- Checks for duplicate names.
- Searches for students.
- Sorts students by name and average.
- Displays student records.

The program also uses custom exceptions to handle invalid grades and students who cannot be found.

 4. Features

- Enter student names and grades for English, Maths, and Science.
- Calculate student averages.
- Check for duplicate names.
- Validate grades.
- Search for students.
- Sort students by name and average.
- Display student reports.

 5. How to Run the Program

1. Install Python and open PyCharm.
2. Save the code as `section_f.py`.
3. Run the program.
4. Enter the number of students, their names, and their grades.

6. Example Output

```text
GRADEBOOK REPORT
--------------------------------------------------
Amahle - Average: 80.00

Enter student name to search: Amahle
Amahle found with average 80.00
```

 7. Testing

The program can be tested by entering valid and invalid grades, adding duplicate names, searching for existing and missing students, and sorting student records.

Actual results should be recorded after testing the program.

8. Assumptions and Limitations

- Grades must be between 0 and 100.
- Student names are case-sensitive.
- Students must have unique names.
- The program stores records temporarily, so data is lost when it closes.
- Bubble sort is used to sort student records.
- Invalid grades are rejected, but the program does not automatically ask the user to enter them again.



  
