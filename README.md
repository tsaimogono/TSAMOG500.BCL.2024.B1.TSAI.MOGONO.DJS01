### DJS01: Mars Climate Orbiter Challenge

The Mars Climate Orbiter incident in 1999 is a stark reminder of the importance of precision in space missions, highlighting how a simple unit mismatch led to the loss of the spacecraft. This challenge seeks to simulate similar challenges in a spacecraft navigation system, emphasising the need for accuracy in calculations.

#### Challenge Overview

This challenge invites students to debug, refactor, and enhance JavaScript functions designed for determining the trajectory of a spacecraft. The initial functions are flawed and may result in incorrect calculations.

![alt text](mars.gif)

##### Problem Areas to Address

1. **Unit Mismatch**: The provided functions fail to convert units correctly, leading to calculation inaccuracies.
2. **Parameter Misalignment**: Parameters are not handled in a way that prevents or highlights the potential for unit mismatch errors, leading to possible confusion.

##### Initial Parameters

- **Initial Velocity (`vel`)**: The starting speed of the spacecraft, 10,000 km/h.
- **Acceleration (`acc`)**: The spacecraft's acceleration, 3 m/s².
- **Time (`time`)**: The duration of the calculation, 3,600 seconds (equivalent to 1 hour).
- **Initial Distance (`d`)**: The starting distance from the reference point, 0 km.
- **Initial Fuel (`fuel`)**: The starting amount of fuel, 5,000 kg.
- **Fuel Burn Rate (`fbr`)**: The rate at which fuel is consumed, 0.5 kg/s.

##### Expected Corrected Results

- **New Velocity**: Approximately 48880 km/h after correction.
- **New Distance**: Approximately 10000 km after correction.
- **Remaining Fuel**: Approximately 3,200 kg after correction.

#### Your Task

1. **Identify and Understand Errors**: Analyse the provided functions to determine how unit mismatches and parameter misalignments cause incorrect results.
2. **Refactor and Correct**: Modify the functions to handle parameters more effectively, incorporating object destructuring for clarity and implementing necessary unit conversions.

#### Solution Approach

- Use object destructuring in function parameters for better clarity.
- Implement accurate unit conversions within the functions.
- Ensure the corrected functions address the issues of unit mismatches and parameter clarity.

#### Debugging Guide

1. Enhance code readability for easier debugging.
2. Identify and correct calculation errors.
3. Improve the robustness of calculations. If incorrect units are used or other errors are detected, the code should notify the user instead of producing an incorrect result.

 # Readme
 
 ## Description
 This script calculates new velocity, new distance, and remaining fuel based on given parameters. It includes error handling for incorrect units of measurement and improves readability.
 
 ## Parameters
 The `props` object contains the following properties:
 - `vel`: Array containing velocity value in km/h and its unit as strings.
 - `acc`: Array containing acceleration value in m/s^2 and its unit as strings.
 - `time`: Array containing time value in seconds and its unit as strings.
 - `d`: Array containing distance value in km and its unit as strings.
 - `fuel`: Array containing fuel value in kg and its unit as strings.
 - `fbr`: Array containing fuel burn rate value in kg/s and its unit as strings.
 
 ## Functions
 ### calcNewVel(props)
 Calculates new velocity based on initial velocity, acceleration, and time. It checks for correct units and throws an error if units are incorrect.
 
 ### newDistance(props)
 Calculates new distance based on initial velocity, time, and initial distance. It checks for correct units and throws an error if units are incorrect.
 
 ### fuelRemaining(props)
 Calculates remaining fuel based on initial fuel, time, and fuel burn rate. It checks for correct units and throws an error if units are incorrect.
 
 ## Usage
 - Call `calcNewVel(props)` to calculate new velocity.
 - Call `newDistance(props)` to calculate new distance.
 - Call `fuelRemaining(props)` to calculate remaining fuel.
 
 ## Debugging
 - Ensure all parameter values have the correct units of measurement.
 - Check the input values and types passed to the functions.
 - Verify the calculations are performed as expected.
 
 ## Output
 - New Velocity: Displays the calculated new velocity in km/h.
 - New Distance: Displays the calculated new distance in km.
 - Remaining Fuel: Displays the calculated remaining fuel in kg.
 
## Feedback

- The code is well-structured and readable.
- Error handling for incorrect units of measurement is helpful for debugging and preventing calculation errors.

## Challenges

- Extend the script to handle different units of measurement (e.g., miles, pounds, gallons) and automatically convert them to the appropriate units before performing calculations.
- Add additional calculations, such as time to reach a certain distance or fuel efficiency.
- Improve error handling to provide more specific error messages for different types of errors (e.g., missing parameters, invalid values).
- Create a user interface to input parameter values and display the results.
