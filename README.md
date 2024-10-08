Car Rental System
Project Overview
The Car Rental System is a menu-driven application that manages customer data, car inventory, lease agreements, and payments. It is built with Java, using object-oriented principles, and interacts with an SQL database to store and retrieve information. The project implements key concepts like control flow statements, exception handling, database interaction, and unit testing.

Features
Customer Management:

Add new customers.
Update customer information.
Retrieve customer details.
Car Management:

Add new cars to the system.
Update car availability.
Retrieve car information.
Lease Management:

Create daily or monthly leases for customers.
Calculate the total cost of a lease based on the type (daily/monthly) and duration.
Retrieve active leases and lease history.
Payment Handling:

Record payments for leases.
Retrieve payment history for a customer.
Calculate the total revenue from payments.
Project Structure
Entity/Model: Contains entity classes representing real-world objects (e.g., Car, Customer, Lease).
DAO: Data Access Object (DAO) interfaces and implementations for interacting with the database.
Exception: Custom exceptions such as CarNotFoundException, CustomerNotFoundException, and LeaseNotFoundException for handling errors.
Util: Utility classes for handling database connection and properties.
Main: Contains the MainModule class, where the application is executed with a menu-driven interface.
Database Schema
Vehicle Table: Contains details about cars available for lease.
vehicleID, make, model, year, dailyRate, status, passengerCapacity, engineCapacity
Customer Table: Stores customer information.
customerID, firstName, lastName, email, phoneNumber
Lease Table: Records details about car leases.
leaseID, vehicleID, customerID, startDate, endDate, type
Payment Table: Manages payments made for leases.
paymentID, leaseID, paymentDate, amount
Setup Instructions
Clone the repository and navigate to the project folder.
Ensure you have the following tools installed:
Java Development Kit (JDK)
MySQL Server
IntelliJ IDEA or another IDE
Configure the SQL database by creating the necessary tables (Vehicle, Customer, Lease, Payment).
Update the DBPropertyUtil class with your database connection details (hostname, username, password).
Run the MainModule class to start the application.
Unit Testing
Unit tests are included for the following scenarios:

Adding a car and verifying its addition.
Creating and retrieving leases.
Handling exceptions when invalid IDs are provided.
How to Run
After setting up the project and database, run the MainModule class.
Follow the prompts in the menu to add customers, cars, create leases, and handle payments.
