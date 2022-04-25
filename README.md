INTRODUCTION

Payroll Management refers to the management of the financial records of the employee . It includes allowances, deductions, bonuses ,etc.
This project ,“Payroll Management System” has been developed keeping in view of the problems faced in the practicing of manual system and  to overcome them .

About the project :

The following are some major concepts that I have used to implement this project:
                        
1.File Handling
2.Pointers
3.OOP Concepts 
4.Width Manipulation
5.Inheritance
6.C++ Graphics, Colours and animations

Following are some features that I have  added in this project:   
1.Colored Interface
2.Guest mode and login page for users
3.Option to go back 
4.Graphics and Animations
5.Data of different departments is kept separate
6.Generates salary as per attendance
7.Generates all components of salary 

MAJOR OPERATIONS PERFORMED 

insert_rec( )
This feature is used to add a new employee record to the department 
It consists of details line name, ID , designation, CTC , attendance ,etc 
It calls the calc( ) function to calculate components based on above inputs

calc( ) 
This function is used to calculate the attendance percentage and the various components of salary including basic( 40%) ,allowance( 45%) and funds(15%) of the CTC . 
It also calculates bonuses and deductions based on attendance.
It finally assigns the calculated salary which an employee gets .

display ( ) 
It displays all the details of employee in a department. If the department is empty , it displays “ No data present”.
It uses C++ width manipulators for displaying the data in tabular form.

search( ) 
It takes the required employee ID as input , compares it with all the employee ids in the department and if that ID is present ,it displays all the details 
If no ID matches , it displays “Employee id not found”
It is used to check the details of a given employee

modify( )
It takes the required employee ID as input , compares it with all the employee ids in the department and if that ID is present ,it only amends that employee detail and rest employees details are copied as they were.
It saves this data in new file and overwrites previous file.
If no ID matches , it displays “Employee id not found”

delete_rec( ) 
It takes the required employee ID as input , compares it with all the employee ids in the department and if that ID is present ,it only deletes that employee detail and rest employees details are copied as they were.
It saves this data in new file and overwrites previous file.
If no ID matches , it displays “Employee id not found”

dispall( )
This function is made available to display all the employee details of different departments at one place .
It displays the records of all employees by calling their respective functions one by one
It calls dispallhelp( ) to call display( ) functions of all classes sequentially

searchall( )
This function is made available to search the employee details of a given employee through all the  departments at once  .
It calls searchhelp( ) to search through each department . 



Other Miscellaneous functions

text_anim ( ) : To add sliding animation

User_login( )  : To create a login interface

Enter_for_continue( )  : To wait for user to press any key to continue
	
Menu( ): To display all menu options

Welcome( ) : Welcome screen for user


Classes used

Class employee_details  :
Contains the data members which are inherited by the Dept classes

Classes Dept1, Dept2 , Dept3… ( max 8) as per number of classes entered by user:
To control manage record of each department separately 

Class alldeplt :
It inherits above 8 classes for displaying and searching through records .


