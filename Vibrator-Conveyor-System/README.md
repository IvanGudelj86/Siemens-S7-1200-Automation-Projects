# Vibrator & Conveyor System

Academic PLC automation project developed in **TIA Portal V15** using a **Siemens S7-1200 CPU 1214C DC/DC/DC**.

The system controls:

- one vibrator drive
- conveyor 1
- conveyor 2

The project demonstrates modular PLC programming, manual and automatic operation, motor speed setpoints, reusable motor-control logic, time-based sequencing and fault handling.

## Program Structure

The main cyclic program calls separate functions for the automatic sequence and individual drives:

- `FC_Auto_Ciklus [FC10]`
- `FC_Vibrator_1 [FC20]`
- `FC_Traka_1 [FC30]`
- `FC_Traka_2 [FC40]`

A reusable motor-control function `sys_FC_MOTOR [FC1]` is used for the vibrator and both conveyor drives.

## Main Functions

### Manual Control

Each drive can be started and stopped individually when automatic mode is not active.

### Automatic Sequence

The automatic cycle coordinates the vibrator and both conveyors and uses time-delay interrupts to control the operating sequence.

### Speed Control

Individual speed setpoints are assigned to the vibrator and conveyor drives. The motor-control function processes the percentage setpoint and scales it to the PLC analog raw-value range.

### Fault Handling

The common motor-control function includes fault logic and status outputs for each controlled drive.

### Data Organization

The project uses Data Blocks and a user-defined motor data type to organize individual drive states and parameters.

## Documentation

The complete TIA Portal program export will be added to the `Documentation` folder.

## Images

Selected LAD networks and project screenshots will be added to the `Images` folder.

## Project Context

This project was completed as a university PLC laboratory exercise and is included as part of a technical automation portfolio.
