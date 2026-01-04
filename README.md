# Automated Conveyor-Based Bottle Filling System 

## Project Overview
This project demonstrates a fully automated conveyor-based bottle filling system designed to improve efficiency, accuracy, and consistency in industrial filling operations.

The system uses an **Arduino Uno** as the control unit, integrating sensors and actuators to automatically detect bottles, stop the conveyor, fill bottles for a fixed duration, and resume conveyor motion without human intervention.

---

## System Objectives
- **Automated Bottle Detection:**  
  Detect the presence of a bottle using an IR sensor mounted along the conveyor line.

- **Sequential Control Logic:**  
  Automatically stop the conveyor, trigger the filling process, and restart movement after filling is complete.

- **Safe Power Interfacing:**  
  Interface high-power components such as motors and solenoid valves with low-power Arduino logic using relays and motor drivers.

---

## Hardware Architecture & Components

### Control & Sensing
- **Arduino Uno** – Central controller
- **IR Sensor** – Bottle detection

### Actuators
- **12V DC Motor** – Drives the conveyor belt
- **Solenoid Valve** – Controls liquid flow during filling

### Power & Interface Electronics
- **L298N Motor Driver** – Motor speed and direction control
- **12V Relay Module** – Switching control for solenoid valve
- **BC547 NPN Transistor** – Relay driving interface
- **1N4007 Diode** – Flyback protection for inductive loads

> System is designed for **12V DC operation** for industrial robustness.

---

## Working Principle
1. The IR sensor detects a bottle on the conveyor.
2. Arduino immediately stops the conveyor motor.
3. The relay activates the solenoid valve.
4. Liquid flows into the bottle for approximately **3 seconds**.
5. The solenoid valve closes.
6. The conveyor restarts and moves the filled bottle forward.

---

## Simulation (Tinkercad)
Due to hardware availability constraints, the complete system logic was tested and validated using a **Tinkercad circuit simulation**.

### Simulation Modifications
- A **9V battery** was used instead of a 12V supply.
- An **LED** was used to represent the solenoid valve operation.
- Since Tinkercad cannot physically move a bottle past a sensor, the IR trigger was simulated using the code.

### Live Simulation Link
 **[View Tinkercad Simulation](https://www.tinkercad.com/things/0XYYqaDD2O0-smashing-vihelmo/editel?returnTo=https%3A%2F%2Fwww.tinkercad.com%2Fdashboard%2Fdesigns%2Fcircuits&sharecode=byqWr3ywkjY6UJrsu6JWklxgMy1SgC1CWiA7I5zb6dM)**

---

##  Repository Structure
 *CONVEYOR BASED BOTTLE FILLING SYSTEM- SIMULATION.pdf
