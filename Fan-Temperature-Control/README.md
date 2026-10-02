# Fan Temperature Control

Academic PLC automation project developed in **Siemens TIA Portal V15** using a **Siemens S7-1200** PLC.

The project demonstrates automatic control of two fans based on a temperature signal, together with modular PLC program organization, time-delay logic and operating counters.

## Main Functions

- Control of two independent fans
- Manual and automatic operating logic
- Temperature signal normalization and scaling
- Temperature threshold comparisons for automatic operation
- Time-delay interrupt logic
- Separate function blocks for each fan
- Operating/start counters using interrupt organization blocks
- Data Blocks for process variables and automatic-cycle data

## Program Structure

The main program calls separate functions for the automatic sequence and both fan drives:

- `FC_Auto_Ciklus` – automatic temperature-based sequence
- `FC_Ventilator_1` – Fan 1 control
- `FC_Ventilator_2` – Fan 2 control
- `sys_FC_TEMP` – temperature normalization and scaling

Additional organization blocks are used for delayed actions and operating counters.

## Temperature Processing

The project contains a reusable temperature-processing function that normalizes an analog input and scales it to the configured engineering range.

Automatic control logic uses temperature thresholds to determine fan operation and delayed activation of the second fan.

## Documentation

- [Full TIA Portal Project Documentation](Documentation/Ventilatori.pdf)

## Project Context

This project was developed as a university laboratory exercise and is included in this repository to demonstrate practical experience with Siemens PLC programming, analog signal processing and automatic control logic.
