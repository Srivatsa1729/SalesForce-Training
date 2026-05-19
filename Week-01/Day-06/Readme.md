1. What is SOQL?

SOQL stands for Salesforce Object Query Language. It is a special query language provided by Salesforce to search, read, and retrieve data from Salesforce objects.

It works similarly to database query languages, but SOQL is specially designed for Salesforce records and relationships.
Using SOQL, users can:
Fetch specific records
Filter required data
Access related object information
Generate reports and results quickly
SOQL is mainly used by developers while writing Apex programs, triggers, and integrations.
Example Usage of SOQL
A college management application may use SOQL to:
Find all students from a particular department
Display students with pending fees
Retrieve attendance information
Show faculty assigned to a course

SOQL helps organizations access data efficiently without manually searching records.

2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that automatically executes when specific actions happen on Salesforce records.

Triggers respond to events such as:

Insert
Update
Delete
Undelete

They help businesses automate backend operations whenever data changes inside the system.
Triggers are useful when automation becomes too advanced for simple Flow-based solutions.

3. Difference Between Flow and Apex Trigger

Flow	Apex Trigger
Created using graphical tools	Developed using programming
Easier for beginners	Requires coding knowledge
Suitable for standard automation	Suitable for complex operations
Faster to configure	Provides greater flexibility
Best for simple workflows	Best for advanced processing
Example
Flow Example:
Automatically sending a fee reminder email.

Trigger Example:
Checking multiple conditions before allowing course registration.

4. Before Trigger vs After Trigger

Before Trigger	After Trigger
Executes before saving data	Executes after data is stored
Used for validation and modifying values	Used for notifications and related operations
Faster because record is not committed yet	Useful for dependent actions
Prevents invalid data from saving	Used when record ID is required
Real-Time Example
Before Trigger:

Automatically calculate student percentage before saving the record.

After Trigger:
Send confirmation email after admission record is created successfully.

5. Trigger Use Cases

1. Student Admission Welcome Message

Trigger Event:
After Insert
Process:

When a new student record is created, the system automatically sends a welcome email containing admission details.

2. Attendance Shortage Notification

Trigger Event:
After Update
Process:

If attendance falls below the required percentage, the system alerts both student and faculty.

3. Course Seat Limit Alert

Trigger Event:
After Update
Process:

When all seats in a course are filled, faculty members receive an automatic notification.

4. Fee Payment Receipt Generation

Trigger Event:
After Update
Process:

After successful fee payment, the system generates a digital receipt automatically.

5. Result Publication Notification

Trigger Event:
After Insert
Process: