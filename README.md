# 🚗 Car Rental Management System (MySQL)

##  Project Title

Car Rental Management System – MySQL Database Design

##  Description

This project is a fully-featured relational database for managing the operations of a car rental company. It allows for storage and tracking of:

* Customers and their license information
* Vehicles, their status, and types
* Rentals and their lifecycle (active, completed, canceled)
* Payments for rentals, including method and status
* Maintenance records for each vehicle

The schema is designed using proper database normalization principles, and includes appropriate data integrity constraints such as primary keys, foreign keys, NOT NULL, UNIQUE, and ENUM types. The relationships model real-world business logic like:

* One-to-Many: A customer can rent many vehicles
* One-to-One: Each rental has one payment
* One-to-Many: Each vehicle can have multiple maintenance records

## ⚙️ How to Run / Setup

1. Clone the repository:

   bash
   git clone [(https://github.com/Meshack-Mesh/Car_rental-database.git)]
   cd car-rental-db

2. Open MySQL or a compatible client (like phpMyAdmin or MySQL Workbench).

3. Import the SQL schema:

   mysql -u your\_user -p < car\_rental\_system.sql

   Or if using MySQL Workbench:

   * Open Workbench
   * Open car\_rental\_system.sql
   * Run the full script to create and set up the database

4. You should now have a database named car\_rental\_system with the following tables:

   * Customers
   * Vehicles
   * Rentals
   * Payments
   * Maintenance

## ERD

ERD Overview:

* One customer → many rentals
* One rental → one payment
* One vehicle → many rentals
* One vehicle → many maintenance records

