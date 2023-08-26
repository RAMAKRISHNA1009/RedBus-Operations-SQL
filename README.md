# RedBus-Operations-SQL

Designing a database for a Red Bus application involves creating a structured system to store and manage various aspects of the application, such as user information, bus routes, bookings, payments, etc. Here's a high-level overview of how you could approach the database design:

# Entities and Relationships:

- Users:
   - User ID (Primary Key)
   - First Name
   - Last Name
   - Email
   - Password
   - Contact Number
   - Address

- Operator ID (Primary Key)
  - Operator Name
  - Contact Information
  - Bus Routes:

- Route ID (Primary Key)
  - Source Location
  - Destination Location
  - Distance
  - Duration
  - Fare
  - Buses:

- Bus ID (Primary Key)
  - Bus Number/Name
  - Operator ID (Foreign Key referencing Bus Operators)
  - Seat Capacity
  - Type (AC, Non-AC, Sleeper, etc.)
   
- Driver ID (Primary Key)
  - Driver Name
  - Contact Number
    
- Booking ID (Primary Key)
  - User ID (Foreign Key referencing Users)
  - Bus ID (Foreign Key referencing Buses)
  - Route ID (Foreign Key referencing Bus Routes)
  - Booking Date
  - Travel Date
  - Number of Passengers
   
- Payments:
  - Payment ID (Primary Key)
  - Booking ID (Foreign Key referencing Bookings)
  - Payment Date
  - Payment Amount
  - Payment Status (Pending, Completed, etc.)
  - Payment Method (Credit Card, Debit Card, etc.)



