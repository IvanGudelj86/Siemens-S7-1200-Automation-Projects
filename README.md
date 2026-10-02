# Siemens S7-1200 Automation Projects

A collection of academic and laboratory PLC automation projects developed using **Siemens S7-1200** controllers and **TIA Portal V15**.

The repository is intended to demonstrate practical experience with PLC programming, modular program organization, automatic sequences, motor control, analog value processing and industrial automation logic.

## Technologies

- Siemens S7-1200
- CPU 1214C DC/DC/DC
- TIA Portal V15
- LAD (Ladder Logic)
- Data Blocks (DB)
- User-Defined Data Types (UDT)
- Time-delay and hardware interrupts
- Analog value scaling
- Automatic and manual operating modes

## Projects

### 1. Vibrator & Conveyor System

PLC control system for one vibrator and two conveyor drives.

Main features:

- Separate control functions for the vibrator and both conveyors
- Manual and automatic operation
- Adjustable motor speed setpoints
- Reusable motor-control function
- Automatic operating sequence using time-delay interrupts
- Fault handling logic
- Analog output scaling from a percentage setpoint to the PLC raw value range

[View project details](Vibrator-Conveyor-System/README.md)

### 2. Fan Temperature Control

PLC control system for two fans based on a temperature signal.

Main features:

- Two independent fan control functions
- Manual and automatic operation
- Temperature normalization and scaling
- Temperature threshold logic
- Time-delay interrupts
- Operating/start counters

[View project details](Fan-Temperature-Control/README.md)

Additional laboratory projects will be added to this repository after review and cleanup.

## Project Context

These projects were developed as university laboratory exercises. They are presented here as a technical portfolio demonstrating practical experience with Siemens PLC programming and industrial automation.

## Author

Ivan Gudelj
