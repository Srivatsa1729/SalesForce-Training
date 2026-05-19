1. Difference Between App, Object, Record, and Field
Term	                                        Explanation
App	                   An App is a complete workspace in Salesforce that brings together 
                        related tools, tabs, and objects for a particular business activity.
Object	               An Object is used to organize and store a particular type of 
                        information, similar to a table in a database.
Record	               A Record is an individual entry stored inside an object. Each record    
                        contains specific details.
Field	               A Field represents a single piece of information within a record.

Simple Example
App:

College Management App

Object:

Student Object

Record:

Srivatsa – CSE – 4th Year

Fields:
Student Name
Branch
Roll Number
Phone Number

2. Standard Objects vs Custom Objects
Standard Objects

Standard Objects are the default objects already available in Salesforce. These are commonly used for customer and business management purposes.

Examples:
Account
Contact
Opportunity
Lead

Custom Objects

Custom Objects are designed by users according to their own business requirements. They allow organizations to build systems based on their workflow.

Examples:
Student
Course
Library
Faculty

3. College Data Model
Objects Used in the System
Student

Stores student-related details such as:

Student Name
Roll Number
Email
Department

Faculty

Maintains faculty information:

Faculty Name
Subject
Experience
Department
Course

Contains course-related data:

Course Name
Duration
Credits
Assigned Faculty
Department

Stores department information:

Department Name
HOD Name
Block Number
Relationships Between Objects
One department can contain multiple students
One department can have several faculty members
A faculty member can handle multiple courses
Multiple students can enroll in the same course

Relationships make the system connected and help avoid duplicate data storage.

Relationship Mapping
Object Relationship	                          Type

Student → Department	                        Lookup Relationship
Faculty → Department	                        Lookup Relationship
Course → Faculty	                            Lookup Relationship
Student → Course	                            Lookup Relationship

College Management System Diagram
Department
   |
   |---- Students
   |
   |---- Faculty
               |
               |---- Courses
                         |
                         |---- Student Enrollments


4. Formula Fields
Student Full Name

A formula field can automatically combine the first name and last name into a single value.

Benefit:

Users do not need to type the full name repeatedly, which reduces spelling mistakes and saves time.

Attendance Percentage

A formula can calculate attendance percentage automatically using:

Classes Attended
Total Classes Conducted
Benefit:

Teachers can instantly monitor student attendance without manual calculations.

Course Fee Balance

This formula calculates the remaining fee amount after payment.

Benefit:

The administration can quickly identify pending payments and maintain accurate financial records.

Available Seats

A formula field can show how many seats are still available in a course.

Benefit:

It helps staff avoid exceeding the maximum admission limit during enrollments.