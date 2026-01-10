# Autonomous RC Car 

## Project Overview

This project documents the design and development of an RC car through multiple hardware and software iterations. Each version added new mechanical, electrical, or software capabilities.

Core features include:
- Brushless motor with ESC
- LiPo battery power system
- Differential drivetrain
- Servo-based steering
- Custom remote control using NRF24L01 transceivers
- Arduino-based control system
- Ultrasonic sensor for autonomous navigation
- Rigid metal chassis (final version)

---

## Iterative Development Stages

### Version 1 – Basic Drive
- Rear-wheel drive
- Brushless motor
- LEGO enclosure
- No steering

### Version 2 – Steering Added
- Servo motor for front-wheel steering
- Manual directional control

### Version 3 – Remote Controlled
- Off-the-shelf RC remote
- Improved drivability

### Version 4 – Custom Remote Control
- NRF24L01 transceivers
- Two Arduino boards (transmitter & receiver)
- Fully custom wireless protocol

### Version 5 – Autonomous Mode
- Ultrasonic distance sensor
- Obstacle detection and avoidance
- Autonomous driving logic

### Version 6 – Final Build
- Metal frame chassis
- Integrated drivetrain, steering, and electronics
- Supports both autonomous and remote-controlled operation

---

## System Architecture

**Electronics:**
- Arduino (control logic)
- NRF24L01 wireless modules
- Ultrasonic sensor (HC-SR04 or similar)
- ESC
- Servo motor
- LiPo battery

**Mechanical:**
- Metal chassis
- Differential drivetrain
- Custom mounts and brackets

---

## Wiring & Power

- LiPo battery powers the ESC and motor
- ESC BEC supplies 5V to Arduino and servo
- NRF24L01 powered via regulated 3.3V
- Ultrasonic sensor powered at 5V


---

## Autonomous Logic (High-Level)

1. Measure distance using ultrasonic sensor
2. If obstacle detected within threshold:
   - Stop
   - Turn servo
   - Resume forward motion
3. Otherwise:
   - Continue forward

---

## Tools & Technologies

- Arduino IDE
- C++
- NRF24L01 wireless protocol
- LiPo power systems

