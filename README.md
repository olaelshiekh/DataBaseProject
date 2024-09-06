# Hotel Management System

![ERD Diagram](https://github.com/olaelshiekh/DataBaseProject/blob/main/ERD_FINAL.PNG)

## Project Overview

This Hotel Management System is designed to manage the key operations of a hotel, such as handling reservations, managing facilities and services, processing payments, and maintaining advertisements. It utilizes a database schema that organizes data related to hotels, customers, employees, services, and reservations.

The project was developed by Ola El-Shiekh at the Faculty of Electronics Engineering, Menofia University, as part of a Level 2 course project.

## Features

- **Facility Management**: Tracks hotel facilities, their types, and costs.
- **Service Management**: Manages various services offered by the hotel, including categories, descriptions, restrictions, and availability.
- **Customer and Employee Data**: Stores customer and employee information, including contact details and position (for employees).
- **Reservation and Booking**: Handles reservations with details such as start/end dates, prices, and associated services or facilities.
- **Advertisements**: Manages advertisement campaigns and their related services or packages.
- **Payments and Charges**: Processes payments and tracks other charges related to bookings.

## Database Schema

The database schema is organized as follows:

1. **Entities**:
    - **Hotel**: Stores details like name, address, country, and contact information.
    - **Facility**: Details of hotel facilities, including capacity and cost.
    - **Service**: Hotel services categorized by type, description, and availability.
    - **Customer**: Stores customer information such as name, address, phone number, and email.
    - **Employee**: Employee data including name, contact details, and position.
    - **Reservation**: Manages reservation details such as start/end date, discount, and customer/employee IDs.
    - **Booking Details**: Specifics about the booking, including date, quantity, and total price.
    - **Advertisement**: Advertisement campaigns including start/end dates, price, and details.
    - **Payment**: Tracks payments for reservations.

2. **Relationships**:
    - **Relation_FacilityType_Service**: Maps facilities to related services.
    - **Relation_Customer_Booking**: Connects customers to their bookings.
    - **Package_Service**: Connects advertisements to their related services.
  
## Database Requirements

- All entities have a primary key.
- Non-null constraints for mandatory fields such as name, address, phone number, and prices.
- Integrity constraints such as checking values (e.g., capacity must be > 0, price must be > 0).
  
## Installation and Setup

1. **Database Setup**:
    - Use the provided SQL DDL (Data Definition Language) statements to create the necessary tables in your database.
    - Ensure you have a suitable database environment (e.g., MySQL, PostgreSQL).

2. **Project Files**:
    - The database schema, SQL queries, and integrity constraints are included in the `schema.sql` file.

3. **Dependencies**:
    - Make sure you have the required database engine installed.
    - SQL client for executing queries.

## Usage

1. **Create Tables**: Execute the provided SQL statements to create tables for managing hotels, services, reservations, etc.
2. **Insert Data**: Populate the tables with relevant data for hotels, customers, services, advertisements, and bookings.
3. **Run Queries**: You can run queries to manage hotel operations like creating bookings, updating services, and generating invoices.

## Contributing

Contributions are welcome! If you have suggestions for improving the system, feel free to submit a pull request or create an issue.


---

This Hotel Management System is a fully-fledged database project that can be expanded and adapted to fit various hotel management needs. Enjoy exploring and building upon it!
