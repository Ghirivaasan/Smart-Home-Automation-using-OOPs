# Smart Home Automation System

## Overview

This project implements a Smart Home Automation System using C++. It allows users to control various smart devices in their home, including lights, thermostats, door locks, security cameras, and smart speakers.

## Features

- Control multiple smart devices from a single interface
- Adjust device settings (e.g., brightness, temperature, volume)
- Save and load device settings from files
- Password-protected access to the system

## Devices

The system includes the following smart devices:

1. **Light**: Control brightness, color, and mode
2. **Thermostat**: Adjust temperature, mode, and humidity
3. **Door Lock**: Lock/unlock, change access code, and bolt/unbolt
4. **Security Camera**: Set resolution, angle, and start/stop recording
5. **Smart Speaker**: Adjust volume, equalizer settings, and bass boost

## Usage

To use the Smart Home Automation System:

1. Compile and run the `main.cpp` file
2. Enter the home access code when prompted (default: "admin@123")
3. Choose a device from the menu
4. Adjust the device settings as needed
5. Settings are automatically saved to individual device files

## Code Structure

The project is organized into several C++ files:

- `main.cpp`: Contains the main program logic and user interface
- `device.cpp`: Defines the base `Device` class
- `light.cpp`: Implements the `Light` class
- `thermostat.cpp`: Implements the `Thermostat` class
- `doorlock.cpp`: Implements the `DoorLock` class
- `securitycamera.cpp`: Implements the `SecurityCamera` class
- `smartspeaker.cpp`: Implements the `SmartSpeaker` class

## Security

The system uses a simple password-based authentication. The default password is set in the `main.cpp` file as "admin@123".

## File Management

Each device saves its settings to a separate text file named after the device (e.g., "Living Room Light.txt"). The system can load these settings when restarting.

## Error Handling

The system implements basic error handling using try-catch blocks to manage invalid inputs and file operations.

## Future Improvements

- Implement a more robust authentication system
- Add support for additional smart devices
- Create a graphical user interface
- Implement network connectivity for remote control
