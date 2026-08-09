# POLARIS – Smart Tracking Device

POLARIS is an ESP32-based embedded system designed to provide direction, GPS-based positioning, and accurate time information in a compact portable device. The system combines a GPS module, magnetometer, RTC, and OLED display with an ESP32 as the main controller.

The project is currently under development. The initial schematic and PCB design have been completed, while PCB refinement and firmware development are the next stages.

## Project Overview

The main objective of POLARIS is to develop a standalone device capable of providing:

* Direction
* Latitude and longitude
* GPS satellite-based time
* Date and time through the RTC when GPS is unavailable

The information will be displayed through a 0.96-inch OLED display. Tactile switches will be used to navigate between different information screens.

## Why POLARIS?

The idea behind POLARIS is to provide essential direction, location, and time information through a small standalone embedded device.

The system is designed to combine multiple sensing modules into a single platform rather than depending on separate instruments for each function.

The project also provides practical experience in embedded systems, sensor interfacing, PCB design, and firmware development.

## Main Features

### Direction Detection

The GY-271 magnetometer is used to detect the Earth's magnetic field and determine the direction of the device. The direction will be displayed on the OLED interface.

### GPS Positioning

The NEO-6M GPS module receives signals from GPS satellites and provides geographical coordinates, including latitude and longitude.

### Satellite-Based Time

GPS satellites provide accurate timing information along with positioning data. POLARIS is designed to use the timing information received through the GPS module as the primary time reference.

### RTC Backup

The DS3231 RTC provides an independent and accurate local time source when GPS signals are unavailable.

### OLED Display

A 0.96-inch OLED display is used to present the information provided by the system. The planned interface includes direction, latitude, longitude, time, and date.

### User Controls

Two tactile switches are included for navigating between different information screens and controlling the display interface.

## Hardware Components

| Component              | Function                                       |
| ---------------------- | ---------------------------------------------- |
| ESP32                  | Main controller and data processing            |
| NEO-6M GPS Module      | Latitude, longitude and GPS timing information |
| GY-271 Magnetometer    | Direction detection                            |
| DS3231 RTC Module      | Backup and local timekeeping                   |
| 0.96-inch OLED Display | Display interface                              |
| 18650 Battery Holder   | Portable power supply                          |
| Tactile Switches       | Screen navigation and control                  |
| Charging Module        | Planned for integration                        |

## System Operation

The NEO-6M GPS module receives signals from GPS satellites and provides latitude, longitude, and timing information.

The GY-271 magnetometer measures the Earth's magnetic field and provides the information required to determine the device's direction.

The ESP32 acts as the central controller. It processes the information received from the GPS and magnetometer and manages the OLED display.

The DS3231 RTC provides timekeeping when GPS signals are unavailable.

The user will be able to view different information through the OLED display using the tactile switches.

## Power Supply

POLARIS is designed to operate using an 18650 battery, allowing the device to be used as a portable system.

A charging module is planned to be integrated into the final hardware design.

## PCB Development

The hardware is being designed using KiCad.

The repository currently contains the project schematic and PCB design files. The initial PCB layout has been developed and is currently being refined before manufacturing.

Current hardware progress:

* Initial schematic completed
* Initial PCB design completed
* PCB refinement in progress
* PCB manufacturing pending
* Hardware assembly pending

## Firmware Development

Firmware development is the next major stage of the project.

The ESP32 firmware will be responsible for:

* Reading GPS data
* Processing latitude and longitude
* Handling GPS timing information
* Reading RTC data
* Processing magnetometer readings
* Determining direction
* Controlling the OLED display
* Managing screen navigation
* Handling tactile switch input

## Project Status

| Development Stage       | Status                    |
| ----------------------- | ------------------------- |
| Project Concept         | Completed                 |
| Component Selection     | Completed                 |
| Schematic               | Initial version completed |
| PCB Design              | In Progress               |
| PCB Refinement          | Pending                   |
| Firmware Development    | Pending                   |
| Sensor Integration      | Pending                   |
| PCB Manufacturing       | Pending                   |
| Hardware Assembly       | Pending                   |
| Testing and Calibration | Pending                   |

## Project Documentation

The repository includes the POLARIS project presentation containing the project overview, hardware components, schematic, PCB layout, 3D PCB visualization, and system description.

### Project Presentation

**POLARIS_Project_Presentation.pptx**

> **Note:** The PowerPoint presentation may not be previewed directly in GitHub. To access the presentation, click the **three-dot menu (⋯)** next to the file and select **Download**. The downloaded `.pptx` file can then be opened using Microsoft PowerPoint or any compatible presentation software.

## Future Development

The remaining development work includes PCB refinement, firmware implementation, sensor integration, PCB manufacturing, hardware assembly, calibration, and complete system testing.

The final objective is to develop a compact standalone device capable of providing direction, latitude, longitude, and accurate time information through a simple OLED interface.

## Project Goal

The goal of POLARIS is to integrate GPS positioning, direction sensing, accurate timekeeping, and a simple user interface into one compact ESP32-based embedded system.

The project is intended to demonstrate the complete development process from component selection and circuit design to PCB development, firmware implementation, hardware assembly, and testing.

## Repository

GitHub: RutvikMakwana1410/Polaris-smart-tracking-device
