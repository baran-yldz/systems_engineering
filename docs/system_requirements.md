# 🚀 Autonomous Drone System – System Requirements

## 1. Overview
This document defines the functional and non-functional requirements for the development of an autonomous UAV (Unmanned Aerial Vehicle) system capable of autonomous navigation, sensor integration, control, and communication via CAN protocol.

---

## 2. Functional Requirements

| ID | Requirement |
|----|-------------|
| FR-01 | The UAV shall be able to take off and land autonomously. |
| FR-02 | The UAV shall follow a predefined GPS-based route. |
| FR-03 | The UAV shall use IMU data to estimate orientation (pitch, roll, yaw). |
| FR-04 | The flight control algorithm shall maintain flight stability using PID control. |
| FR-05 | The system shall monitor battery status and perform emergency landing when critically low. |
| FR-06 | Sensor data shall be transmitted over a CAN bus. |
| FR-07 | The system shall enter Safe Mode upon sensor malfunction detection. |

---

## 3. Hardware Requirements

- ARM-based 32-bit microcontroller
- IMU sensor (e.g., MPU6050 or BMI160)
- GPS module with NMEA output
- Brushless motors with ESCs
- CAN transceiver (e.g., MCP2551)
- LiPo battery (11.1V or 14.8V recommended)

---

## 4. Software Requirements

- Programming Language: C++ (OOP structured)
- RTOS: FreeRTOS (optional)
- Modeling Tools: SysML / UML (Use Case, BDD, Sequence, Activity diagrams)
- Simulation Tools: MATLAB / Simulink (flight dynamics, PID tuning)
- Communication Protocol: CAN 2.0B (CANopen or custom frame format)
- Version Control: Git (GitHub repository)

---

## 5. System Features

- Modular flight controller software
- Sensor fusion (IMU + GPS) with Kalman Filter
- Real-time CAN messaging between modules
- Simulink-based model-in-the-loop testing
- Safety fallback logic for critical failures

---

## 6. Constraints

- Max weight: 2.5 kg
- Max flight time: 15 minutes
- Operating temperature: -10°C to +50°C
- All code must be real-time safe (no blocking delays)

---

## 7. Glossary

| Term | Description |
|------|-------------|
| UAV | Unmanned Aerial Vehicle |
| IMU | Inertial Measurement Unit |
| PID | Proportional-Integral-Derivative control algorithm |
| CAN | Controller Area Network |
| RTOS | Real-Time Operating System |
