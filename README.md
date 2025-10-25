# Smart Helmet for Accident Prevention — An EV-Based Approach

This repository contains the source code and header files for our project Smart Helmet for Accident Prevention.  
The project focuses on integrating rider safety features into an electric vehicle (EV) using Arduino-based embedded systems.

---

## 🧠 Project Overview

Road accidents are a major global concern, and many fatalities occur due to riders not wearing helmets or driving under unsafe conditions.  
This project proposes a **Smart Helmet** system that integrates multiple sensors and communication modules to ensure rider safety and prevent accidents.  
The system is divided into two main units:
- Helmet Module
- Bike Module

These modules communicate wirelessly using a ZigBee interface.



# Features

- Helmet Detection: Ensures the rider is wearing the helmet using a force sensor.  
- Alcohol Detection: Uses an MQ-2 gas sensor to detect alcohol levels before allowing the bike to start.  
- Voice Monitoring: Uses a microphone to detect when the rider is talking, automatically reducing vehicle speed to prevent distraction.  
- Fingerprint Authentication: Allows only authorized users to start the vehicle (anti-theft mechanism).  
- Accident Detection:Vibration sensor triggers GPS and GSM modules to alert emergency contacts in case of a crash.  
- Real-time Tracking: GPS module provides live location tracking of the bike.



#Hardware Components

- Arduino Uno / Mega microcontroller  
- R305 Fingerprint Sensor  
- MQ-2 Gas Sensor  
- Force Sensor  
- Microphone Module  
- Vibration Sensor  
- GSM & GPS Modules  
- ZigBee Transceiver  
- Brushless DC Motor (for EV control)  
- 16x2 LCD Display  
- L293D Motor Driver IC  



#Software and Tools

- Arduino IDE — For embedded C programming and debugging  
- Proteus Pro — For simulation and circuit design  
- Embedded C — For developing firmware logic  



# Repository Structure

| File Name         | Description |
|--------------------|-------------|
| `ITWI02_RX.ino`    | Receiver section — handles bike module logic, including fingerprint, GPS, GSM, and data reception. |
| `ITWI02_TX.ino`    | Transmitter section — handles helmet module logic, including force, gas, and microphone sensors. |
| `fingermatch.h`    | Header file for fingerprint sensor functions. |
| `gps.h`            | Header file for GPS module configuration. |
| `gsm.h`            | Header file for GSM communication. |
| `mic_sensor.h`     | Header file for microphone input and processing. |


# Testing and Results

- Simulation: Conducted in Proteus for circuit validation.  
- Hardware Testing: The system successfully authenticated users, monitored helmet usage, and detected accident conditions.  
- Accident Scenario: Automatically sent SMS with live GPS coordinates via GSM.  
- Voice Detection: Effectively reduced motor speed during rider conversation.  



# Conclusion

The Smart Helmet system effectively combines rider authentication, accident prevention, and real-time monitoring.  
By integrating these technologies into an **electric vehicle (EV)**, the project promotes sustainable and safe transportation.  



