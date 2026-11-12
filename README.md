# Beauty Salon Database

A relational database project for managing a beauty salon's customers, employees, services, and appointments.

## Project Overview

The database is named `BeautySalonDB` and is created using SQL. It organizes salon information into related tables and includes sample records and queries.

## Database Tables

- **Customer**: stores customer IDs, names, phone numbers, and email addresses.
- **Employee**: stores employee IDs, names, specialties, and phone numbers.
- **Service**: stores service names, prices, and durations.
- **Appointment**: stores appointment dates, times, statuses, and the related customer and employee.
- **Appointment_Service**: connects appointments with the services selected for them.

## Features and SQL Concepts

- Primary keys and foreign keys.
- `CHECK` constraints for service prices, durations, and appointment statuses.
- Sample data using `INSERT`.
- Queries to display completed appointments.
- `MIN()` and `MAX()` to find the lowest and highest service prices.
- `JOIN` queries to display appointment, customer, and employee details.
- A subquery to list customers with completed appointments.
- A view named `AppointmentReport` that combines appointment, customer, employee, and service information.

## Technologies Used

- SQL
- Relational database concepts

## Files

```text
BeautySalonDB/
├── README.md
└── BeautySalon.sql
```

## How to Run

1. Open your SQL database management tool (for example, MySQL Workbench, if your server supports this script).
2. Open `BeautySalon.sql`.
3. Execute the script.
4. Refresh the database/schema list and check for `BeautySalonDB`.
5. Run `SELECT * FROM AppointmentReport;` to view the report.

## Important Notes

- The script starts by dropping `BeautySalonDB` if it already exists, then creates it again. **Running the script again will delete the existing database with the same name and recreate it**, so back up any important data first.
- The SQL file uses common SQL syntax. Some details may need adjustment depending on the database system you use.
