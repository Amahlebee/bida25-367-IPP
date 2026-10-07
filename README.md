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
 Section C also allows the user to view all grades for a particular subject across the entire class. The program uses a for loop with .items() to go through each student's name and grades.
 The program also includes a search feature that allows the user to enter a student's name and retrieve their grades and average. The program first checks whether the student exists using if search in students:. If the student is found, their grades are retrieved and their average is calculated
 
