# Vehicle Management System

## Overview

The Vehicle Management System is a C++ application designed to manage vehicle details, add new vehicles, update existing ones, and handle user login. The project uses file handling for data storage and retrieval, allowing users to interact with the system through a console interface. It utilizes standard input/output streams to read/write vehicle data.

## My Contributions

- **Add Vehicle**: Add new vehicle details to the system.
- **Search Vehicle**: Search for vehicles by their registration number or other attributes.
- **Update Vehicle**: Modify existing vehicle details.
- **Delete Vehicle**: Remove vehicle information from the system.
- **List All Vehicles**: Display all vehicles stored in the system.

## Code Structure

- **Vehicle Class**: Encapsulates all details about a vehicle, including attributes like registration number, owner, model, and more.
- **File Handling**: Utilizes file streams (`ifstream`, `ofstream`, `fstream`) for data persistence. All vehicle data is stored in a text file and managed via the application.
- **User Interaction**: The program includes a menu-driven console interface where users can interact with the system.

### Functions

1. **addVehicle()**: Prompts the user to input vehicle details and saves them into the file.
2. **searchVehicle()**: Searches for a vehicle in the file based on the registration number and returns its details.
3. **updateVehicle(int regNum)**: Updates the information of a specific vehicle in the file.
4. **deleteVehicle(int regNum)**: Removes a vehicle’s details from the file.
5. **listVehicles()**: Displays all the vehicles stored in the file.

## Technologies Used

- **C++**: For the core logic and functionality.
- **File Handling**: For persistent data storage of vehicle information.
- **Standard Input/Output Streams**: For interaction with the user.
  
## Requirements

- C++ compiler (such as `g++`).

## How to Compile and Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Arjit1512/vehicle-management-system.git
   ```
2. **Navigate to the Directory**:
   ```bash
   cd vehicle-management-system
   ```
3. **Compile the Code**:
   Use a C++ compiler to compile the code. For example, with `g++`:
   ```bash
   g++ -o VehicleManagementSystem vehicle.cpp
   ```
4. **Run the Program**:
   After compiling, run the executable:
   ```bash
   ./VehicleManagementSystem
   ```

## Example Usage

1. **Add a Vehicle**:
   ```
   Enter Vehicle Registration Number: KA05AB1234
   Enter Owner Name: John Doe
   Enter Model: Honda City
   Enter Year of Manufacture: 2018
   Vehicle Added Successfully!
   ```

2. **Search for a Vehicle**:
   ```
   Enter Vehicle Registration Number to Search: KA05AB1234
   Vehicle Found:
   Registration Number: KA05AB1234
   Owner: John Doe
   Model: Honda City
   Year: 2018
   ```

3. **Update Vehicle Information**:
   ```
   Enter Registration Number to Update: KA05AB1234
   Enter New Owner Name: Jane Doe
   Vehicle Updated Successfully!
   ```

4. **Delete a Vehicle**:
   ```
   Enter Registration Number to Delete: KA05AB1234
   Vehicle Deleted Successfully!
   ```

5. **List All Vehicles**:
   ```
   Registration Number: KA05AB1234, Owner: John Doe, Model: Honda City, Year: 2018
   Registration Number: KA04XY9876, Owner: Alice Smith, Model: Toyota Corolla, Year: 2019
   ```
