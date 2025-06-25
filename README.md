# About Me
I'm passionate about data analysis and enjoy solving real-world problems through structured thinking and SQL logic. 
This project reflects my first step into the data domain and showcases my interest in working with data-driven decision-making.
I’m looking forward to building more projects like this in the data analytics and data science field.


✈️ Airline Management System – DBMS Project

📘 Course: Database Management System (IT214)  
Group: 5
Group Representative:  
- Bavarva Megh Dineshbhai (202301402) – 📞 8849855886

Team Members:  
- Patel Naman Vipulbhai (202301423)  
- Patel Het Jitendrakumar (202301421)



#Project Overview
This project simulates an Airline Management System with a focus on real-world processes such as flight bookings, check-ins, meal preferences, payment tracking, and crew assignments. 
The goal is to model and normalize the database schema up to **BCNF** and run complex SQL queries to extract business insights.


## Description

The system handles the following core modules:
1. Passenger registration and loyalty tracking
2. Booking and check-in management
3. Flight and aircraft details
4. Crew and employee assignments
5. Meal preferences and dietary options
6. Luggage tracking
7. Payment processing and currency handling
8. Airport and terminal information
9. Customer reviews and ratings




## Schema Design

The schema includes the following entities:
- Passenger
- Loyalty
- Booking
- Check-in
- Luggage
- Meals
- Payments
- Flights
- Airports
- Terminals
- Aircraft
- Employee
- Crew
- Review

Each table is designed with clear primary keys and foreign key relationships, enabling data integrity and smooth query operations.


## Functional Dependencies

Functional dependencies were derived for all relations. For example:
- `p_id → First_Name, Middle_Name, Last_Name, DOB, ...`
- `booking_id → source, destination, flight_id, meal_id, ...`
- `flight_id → flight_no, departure_time, arrival_time, ...`
- `payment_id → amount, currency, booking_id, loyalty_id`

Full details are provided in the attached relational schema document.



## Normalization

All relations are normalized to **Boyce-Codd Normal Form (BCNF)**. For each table:
- There are no partial or transitive dependencies
- Every functional dependency has a superkey on the left-hand side
- All attributes are fully functionally dependent on the primary key

This ensures minimal redundancy and optimal structure for query performance.



## Sample Analytical Queries

The project includes a set of SQL queries to derive business insights:

- Identify top 10 spending passengers
- List flights with more than 80% seat occupancy
- Highlight premium passengers spending above average
- Track crew assigned to multiple flights in a day
- Compare domestic vs international flight ratings
- Calculate revenue grouped by flight and currency
- Analyze average flight duration by aircraft model
- Determine the most frequent flight route
- Detect passengers with complex itineraries
- Correlate crew experience with flight ratings

These queries demonstrate the practical utility of the database and were tested using PostgreSQL.


# Future Improvements

- Create a front-end interface using Flask or Streamlit
- Add stored procedures for common operations
- Visualize analytics using charts or dashboards
- Implement backup and recovery scripts


# License
This project is created for educational purposes under the DBMS course at university level.
