# Taxi and Shuttle Management System
This is a small, independent project designed to help a taxi company manage its fleet of vehicles, which includes both taxis and shuttles. The system allows for tracking and managing bookings, calculating fares, and generating a daily report in a text file format. Taxis and shuttles have distinct fare structures, which this system accounts for when calculating journey prices and preparing reports.

# Project Structure
Vehicle Classes
The project involves two main vehicle types, Taxi and Shuttle, both of which inherit from a base vehicle class. Each vehicle has an ID and a list of bookings.

Taxi Class

The Taxi class is designed for individual taxis, each with its own:

- Fixed Fare (int): A unique journey price in whole pounds, set per taxi.
- Driver Name (String): The name of the driver assigned to the taxi.
- ID (int): A unique identifier for each taxi.
- Bookings (List): A list that records each booking made for this taxi.
  
Key functionalities for this class may include adding bookings and calculating the total fares for the day based on each taxi’s fixed fare.

Shuttle Class

The Shuttle class represents shuttles that operate on a circular route, where fares are calculated based on the number of stops. Each shuttle has:

- Cost per Stop (int): The fare charged per stop travelled, which varies depending on the shuttle's route characteristics.
- Route Stops (List<String>): A circular list of stop names along the shuttle’s route.
- ID (int): A unique identifier for each shuttle.
- Bookings (List): A list that records each booking made for this shuttle.
  
The shuttle class includes methods for booking journeys and calculating journey prices based on the number of stops travelled, which is determined by the start and end points of each journey.

# Daily Reporting

The system generates a daily report at the end of each day that includes the following information:

- Taxi and Shuttle Summaries: A list of each vehicle with details of its bookings, journey fares, and total earnings for the day.
- Booking Summaries: Detailed breakdowns of bookings for each vehicle, including routes taken, journey costs, and total fares.
  
The report is generated in a text file format, providing the company with an overview of daily operations and earnings.

# Features

- Taxi and Shuttle Fare Management: Supports both fixed fares (for taxis) and per-stop fares (for shuttles).
- Flexible Booking System: Allows bookings for each vehicle type and calculates fares based on each vehicle’s pricing structure.
- Daily Reporting: Generates a text file summary of all bookings, fares, and total earnings for the day.
- Independent Design: This project is self-contained, suitable for independent use by a taxi company, but could be expanded or integrated into larger fleet management systems.
