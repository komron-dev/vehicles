# Vehicle Management System

This project is a Java-based application for managing different types of vehicles, such as cars, trucks, and buses. The system allows users to perform various operations such as adding, removing, and listing vehicles, along with handling invalid inputs via custom exceptions.

## Features

- **Vehicle hierarchy**: The project includes a base `Vehicle` class, with specific subclasses like `Car`, `Truck`, and `Bus`.
- **Custom Exception Handling**: Implements an `InvalidInputException` for handling user input errors.
- **Vehicle Database**: A `Database` class for storing and managing vehicles.
- **Console-based User Interaction**: The `Main` class provides a simple console interface to interact with the vehicle database.

## Project Structure

```bash
vehicles/
│
├── Bus.java                # Class representing a bus
├── Car.java                # Class representing a car
├── Database.java           # Class for managing a collection of vehicles; reads input data from file
├── InvalidInputException.java  # Custom exception class for invalid inputs
├── Main.java               # Entry point of the application
├── Truck.java              # Class representing a truck
└── Vehicle.java            # Base class for all vehicle types
```
