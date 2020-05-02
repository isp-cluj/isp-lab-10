# Air Traffic Control System

In this lab you will implement a simplified air traffic control (ATC) sistem which allow user to add airplains and controll them.

## Use Case Diagram
![Exercise 1 image](docs/UseCaseDiagram1.jpg)

## Aircraft State Machine Diagram
![Exercise 2 image](docs/StatechartDiagram1.jpg)

## ATC Class Diagram
![Exercise 1 image](docs/ClassDiagram1.jpg)

## Requirements

- R1 - When aircraft receives takeoff command will go into Taxing state and will stay there for 10 seconds; 
- R3 - Take off command contains cruising altitude for the aircraft;
- R2 - From Taxing aircraft will go into Taking off state and will stay there for 5 seconds;
- R3 - Aircraft will stay in Ascending state till airplain reach cruising altitude. Altitude is given by ATC in 1.000 meters increments and needs 10 seconds for each incremet. Example: altitude 3 = means airplain cruising altitude is 3.000 meters.
- R4 - Aircraft can receive land command only when is at cruising altitude;
- R5 - Descending logic is the same as for ascending (see R3);
- R6 - When aircraft has reached altitude 0 is considered landed;
- R9 - User interaction is done trough a console based user interface (read commands from keyboard); 
- R10 - Aircrafts are implemented as threads;
- R11 - Aircraft will keep track of number of seconds spent in "Cruising" state and will display it after it landed;
- [OPTIONAL] - Add a graphical user interface to let user ineract wit ATC system;

