PROJECT OVERVIEW :
Classes:
1. Passenger: Represents a passenger with attributes like name, age, and passenger class (economy or business).
2. Flight: Represents a flight with attributes like flight number, destination, distance, fuel required, and a list of passengers.
3. AirlineManagementSystem: Manages a list of flights and provides methods for adding, displaying, searching, deleting, and updating flights, as well as adding passengers to flights.
Methods:

1. addFlight(): Adds a new flight to the system.
2. displayAllFlights(): Displays all flights in the system.
3. searchFlight(): Searches for a flight by flight number.
4. deleteFlight(): Deletes a flight from the system.
5. updateFlight(): Updates the details of a flight.
6. addPassengerToFlight(): Adds a passenger to a flight.

Main Function:

The main function implements a simple menu-driven interface for the user to interact with the Airline Management System. It repeatedly prompts the user to choose an option (add flight, display all flights, search flight, delete flight, update flight, add passenger to flight, or exit) and calls the corresponding method.

Login Function:

The login() function is a simple authentication mechanism that checks if the user enters the correct username and password (hardcoded as "admin" and "password", respectively).

Overall, this code provides a basic implementation of an Airline Management System, allowing users to manage flights and passengers.
KEY FEATURES:
1. Class Definitions and Encapsulation:
Flight Class:
  - Stores flight details like flight number, destination, distance, fuel required, and passengers.
  - Methods:
    - setData: Sets flight details.
    - showData: Displays flight details including passenger details.
    - getFlightNumber: Returns the flight number.
  - Contains a friend class declaration allowing AirlineManagementSystem to access its private members.

Passenger Class:
  - Stores passenger details like name, age, and class (Economy or Business).
  - Methods:
    - setData: Sets passenger details.
    - showData: Displays passenger details.
2. AirlineManagementSystem Class:
- Manages multiple flights and operations related to flights and passengers.
- Attributes:
  - An array of Flight objects (flights) with a maximum size defined by MAX_FLIGHTS.
  - numFlights to keep track of the number of flights.
- Methods:
  - addFlight: Adds a new flight if the maximum limit is not reached.
  - displayAllFlights: Displays details of all flights.
  - searchFlight: Searches for a flight by flight number and displays its details.
  - deleteFlight: Deletes a flight by flight number.
  - updateFlight: Updates details of an existing flight.
  - addPassengerToFlight: Adds a passenger to a specific flight if the flight is found and has available passenger slots.
3. Login Functionality:
- A simple login system that checks for a hardcoded username and password.
- If login fails, the program exits.

4. User Interface and Interaction:
- Uses a console-based menu to interact with the user.
- Allows the user to:
  - Add a flight.
  - Display all flights.
  - Search for a specific flight.
  - Delete a flight.
  - Update flight details.
  - Add a passenger to a flight.
  - Exit the program.
5. Predefined Constants:
- MAX_FLIGHTS and MAX_PASSENGERS: Define the maximum number of flights and passengers per flight, respectively.
- ECONOMY and BUSINESS: Define passenger class types.
 6.Main Function:
- Displays a welcome message and performs a login check.
- If login is successful, it presents a menu-driven interface for performing various operations on the flights and passengers.

7. Error Handling and User Prompts:
- Checks for conditions like maximum number of flights or passengers being reached.
- Prompts the user for required input and provides feedback on operations performed (e.g., flight added, flight not found).

8.System Calls and Aesthetics:
- Uses system("color 80") and Sleep(2000) for visual effects in the console (specific to
