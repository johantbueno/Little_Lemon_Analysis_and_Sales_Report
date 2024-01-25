# Little_Lemon_Analysis_and_Sales_Report
About the Project:  Little Lemon is a family-owned Mediterranean restaurant. They are developing a Python-based application that needs to connect with the MySQL database so that the booking, menu, and order data can be stored in the respective tables.
Database Clients Project

The following Software and Packages are installed for completing this project :

Python

MySQL server

Jupyter notebook

MySQL Connector/Python API

About the Project:

Little Lemon is a family-owned Mediterranean restaurant. They are developing a Python-based application that needs to connect with the MySQL database so that the booking, menu, and order data can be stored in the respective tables.

The restaurant owner wants to use the stored data to make data-driven decisions to increase their revenue. Establishing a database is one of their key objectives.

The given steps are used to set up the Little Lemon database:

Step 1: Establish a connection:

Open a new Jupyter notebook and import the MySQL Connector/Python API to establish a connection between Python and MySQL database.

Step 2: Create a cursor:

Once the connection between Python and MySQL database is successfully established, you need a cursor object to communicate with MySQL.

Step 3: Create the database and set it for use:

Now that you have a connection and a cursor, create a new database little_lemon_db, and set the database for use.

Step 4: Create tables and Insert data:

Create and populate the tables in the little_lemon_db database: MenuItems table, Menu table, Bookings table, Orders table, and Employees table.

Step 5: Implement and query stored procedures:

Create a pool of connections and get a connection from the pool to implement the stored procedures to complete the following tasks:

Establish a connection by importing MySQLConnectionPool and creating a pool with two connections.

Create and call a stored procedure named PeakHours that identifies the peak, or busiest hour, for the restaurant based on the number of bookings.

Create and call a stored procedure named GuestStatus that outputs the status of each guest’s order based on which employee is assigned to the order.

Stored procedures are created to carry out routine operations on MySQL databases. They are consistent and make sure that the written SQL queries in the procedures are executed in the same way every time you call the stored procedure. A stored procedure is created only once, and you store it in the MySQL database. You can call the stored procedures as many times as you need in a Python-based application.

The tasks and the steps that you must follow to complete each one are as follows:

Task 1: Establish a connection

Step one: Import MySQLConnectionPool

Step two: Import Error

Step three: Create a pool named pool_a with two connections. Use a try-except block to handle any possible errors.

Step four: Obtain a connection from pool_a and create a cursor object to communicate with the database.

Task 2: Implement a stored procedure called PeakHours

Step one: Write a SQL CREATE PROCEDURE query for PeakHours

Use HOUR to extract the hour part from the BookingSlot.

Use COUNT to count the number of bookings.

Use GROUP BY on booking hour.

Use ORDER BY on the number of bookings in descending order.

Step two: Run the stored procedure query by invoking execute module on the cursor.
