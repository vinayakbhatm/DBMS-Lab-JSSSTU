# DBMS-Lab-JSSSTU
##Sailors Database

Write ER diagram and schema diagram. The primary keys are underlined and the data types are specified. Create tables for the following schema listed below by properly specifying the primary keys and foreign keys. Enter at least five tuples for each relation.

Sailors database
SAILORS (sid, sname, rating, age)
BOAT(bid, bname, color)
RSERVERS (sid, bid, date)
Queries, View and Trigger

Find the colours of boats reserved by Albert
Find all sailor id’s of sailors who have a rating of at least 8 or reserved boat 103
Find the names of sailors who have not reserved a boat whose name contains the string “storm”. Order the names in ascending order.
Find the names of sailors who have reserved all boats.
Find the name and age of the oldest sailor.
For each boat which was reserved by at least 5 sailors with age >= 40, find the boat id and the average age of such sailors.
Create a view that shows the names and colours of all the boats that have been reserved by a sailor with a specific rating.
A trigger that prevents boats from being deleted If they have active reservations.


##Insurance Database
Consider the database schemas given below. Write ER diagram and schema diagram. The primary keys are underlined and the data types are specified. Create tables for the following schema listed below by properly specifying the primary keys and foreign keys. Enter at least five tuples for each relation.
Insurance database

PERSON (driver id#: string, name: string, address: string)
CAR (regno: string, model: string, year: int)
ACCIDENT (report_ number: int, acc_date: date, location: string)
OWNS (driver id#: string, regno: string)
PARTICIPATED(driver id#:string, regno:string, report_ number: int,damage_amount: int)
Queries, View and Trigger

Find the total number of people who owned cars that were involved in accidents in 2021.
Find the number of accidents in which the cars belonging to “Smith” were involved.
Add a new accident to the database; assume any values for required attributes.
Delete the Mazda belonging to “Smith”.
Update the damage amount for the car with license number “KA09MA1234” in the accident with report.
A view that shows models and year of cars that are involved in accident.
A trigger that prevents a driver from participating in more than 3 accidents in a given year.


##Order Processing Database
3.Write ER diagram and schema diagram. The primary keys are underlined and the data types are specified. Create tables for the following schema listed below by properly specifying the primary keys and foreign keys. Enter at least five tuples for each relation. Order processing database

Customer (Cust#:int, cname: string, city: string)
Order (order#:int, odate: date, cust#: int, order-amt: int)
Order-item (order#:int, Item#: int, qty: int)
Item (item#:int, unitprice: int)
Shipment (order#:int, warehouse#: int, ship-date: date)
Warehouse (warehouse#:int, city: string)
Queries, View and Trigger

List the Order# and Ship_date for all orders shipped from Warehouse# "W2".
List the Warehouse information from which the Customer named "Kumar" was supplied his orders. Produce a listing of Order#, Warehouse#.
Produce a listing: Cname, #ofOrders, Avg_Order_Amt, where the middle column is the total number of orders by the customer and the last column is the average order amount for that customer. (Use aggregate functions)
Delete all orders for customer named "Kumar".
Find the item with the maximum unit price.
A tigger that updates order_amount based on quantity and unit price of order_item .
Create a view to display orderID and shipment date of all orders shipped from a warehouse 5.


##Enrollment Database
4.Write ER diagram and schema diagram. The primary keys are underlined and the data types are specified. Create tables for the following schema listed below by properly specifying the primary keys and foreign keys. Enter at least five tuples for each relation.

Student enrollment in courses and books adopted for each course

STUDENT (regno: string, name: string, major: string, bdate: date)
COURSE (course#:int, cname: string, dept: string)
ENROLL(regno:string, course#: int,sem: int,marks: int)
BOOK-ADOPTION (course#:int, sem: int, book-ISBN: int)
TEXT (book-ISBN: int, book-title: string, publisher: string,author: string)
Queries, View and Trigger

Demonstrate how you add a new text book to the database and make this book be adopted by some department.
Produce a list of text books (include Course #, Book-ISBN, Book-title) in the alphabetical order for courses offered by the ‘CS’ department that use more than two books.
List any department that has all its adopted books published by a specific publisher.
List the students who have scored maximum marks in ‘DBMS’ course.
Create a view to display all the courses opted by a student along with marks obtained.
Create a trigger that prevents a student from enrolling in a course if the marks pre_requisit is less than the given 40 .


##Company Database
5.Write ER diagram and schema diagram. The primary keys are underlined and the data types are specified. Create tables for the following schema listed below by properly specifying the primary keys and foreign keys. Enter at least five tuples for each relation.

Company Database:

EMPLOYEE (SSN, Name, Address, Sex, Salary, SuperSSN, DNo)
DEPARTMENT (DNo, DName, MgrSSN, MgrStartDate)
DLOCATION (DNo,DLoc)
PROJECT (PNo, PName, PLocation, DNo)
WORKS_ON (SSN, PNo, Hours)
Queries, View and Trigger

Make a list of all project numbers for projects that involve an employee whose last name is ‘Scott’, either as a worker or as a manager of the department that controls the project.
Show the resulting salaries if every employee working on the ‘IoT’ project is given a 10 percent raise.
Find the sum of the salaries of all employees of the ‘Accounts’ department, as well as the maximum salary, the minimum salary, and the average salary in this department
Retrieve the name of each employee who works on all the projects controlled by department number 5 (use NOT EXISTS operator).
For each department that has more than five employees, retrieve the department number and the number of its employees who are making more than Rs. 6,00,000.
Create a view that shows name, dept name and location of all employees.
Create a trigger that prevents a project from being deleted if it is currently
