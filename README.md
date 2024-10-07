# Vehicle Refuel Management System

This Java-based project processes a text file containing refueling data for different types of vehicles (cars, trucks, and buses). The application calculates various statistics, such as the average number of refuels per vehicle, and identifies the vehicle that was refueled the most and the least in terms of both fuel amount and the number of refueling events, categorized by vehicle type.

## Features

- **File-based Input**: Reads a text file containing refueling data for cars, trucks, and buses.
- **Vehicle Refueling Statistics**:
  - Calculates the mean number of refuels per vehicle.
  - Identifies the vehicle refueled the least and the most based on fuel amount and refuel events, within each vehicle category (Car, Bus, Truck).
- **Vehicle Categories**: Supports three types of vehicles:
  - `C` - Car
  - `B` - Bus
  - `T` - Truck

## Input File Format

The input file follows this format:


1. The first line contains an integer `n`, which represents the number of vehicles.
2. The following `n` lines each contain:
   - The vehicle type (`C` for Car, `B` for Bus, `T` for Truck)
   - The license plate number (e.g., `AAA-111`)
   - The number of refuels
   - The list of refuel amounts

### Example File
```
3 C AAA-111 4 6 7 8 9
B ABC-123 2 3 13
T FFF-888 7 1 2 3 4 5 6 7
```

In this example:
- Car `AAA-111` was refueled 4 times with amounts: 6, 7, 8, and 9.
- Bus `ABC-123` was refueled 2 times with amounts: 3 and 13.
- Truck `FFF-888` was refueled 7 times with amounts: 1, 2, 3, 4, 5, 6, and 7.

## Project Structure

```bash
vehicles/
│
├── Bus.java                # Class representing a bus
├── Car.java                # Class representing a car
├── Database.java           # Class for managing vehicle data and refuels; reads data from file
├── InvalidInputException.java  # Custom exception class for invalid inputs
├── Main.java               # Entry point of the application
├── Truck.java              # Class representing a truck
└── Vehicle.java            # Base class for all vehicle types
