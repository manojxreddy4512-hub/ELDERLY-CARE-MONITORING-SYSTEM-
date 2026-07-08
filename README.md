# ELDERLY-CARE-MONITORING-SYSTEM-
Developed an IoT-based Elderly Care Monitoring System using ESP32, MPU6050, and GPS for real-time fall detection, location tracking, medicine reminders, and emergency alerts. Built a web dashboard for live remote monitoring, improving elderly safety and caregiver response.

# Elderly Care Monitoring System

## Overview

The Elderly Care Monitoring System is an IoT-based project developed to improve the safety and well-being of senior citizens. The system uses an ESP32 microcontroller with an MPU6050 motion sensor and a GPS module to detect falls and track the user's location in real time. A built-in web dashboard allows caregivers to monitor the user's status remotely, while a medicine reminder and emergency buzzer provide additional support. :contentReference[oaicite:0]{index=0}

## Features

- Real-time fall detection using MPU6050
- GPS-based live location tracking
- ESP32 web dashboard for remote monitoring
- Emergency buzzer alert
- Push button to cancel false alarms
- Medicine reminder
- Wi-Fi-based communication
- Real-time status updates

## Hardware Components

- ESP32 Development Board
- MPU6050 Accelerometer and Gyroscope
- GPS Module (NEO-6M)
- Active Buzzer
- Push Button
- Breadboard
- Jumper Wires
- USB Cable

## Software Requirements

- Arduino IDE
- ESP32 Board Package
- TinyGPS++ Library
- Adafruit MPU6050 Library
- Adafruit Sensor Library
- WiFi Library
- WebServer Library

## Circuit Connections

### MPU6050

VCC → 3.3V

GND → GND

SDA → GPIO 21

SCL → GPIO 22

INT → GPIO 19

### GPS Module

VCC → 5V

GND → GND

TX → GPIO 16

RX → GPIO 17

### Buzzer

Positive → GPIO 18

Negative → GND

## Working

1. ESP32 initializes the MPU6050 and GPS modules.
2. Motion data is continuously monitored.
3. If abnormal acceleration exceeds the threshold, a fall is detected.
4. The buzzer is activated to alert nearby caregivers.
5. The user can stop the alarm using the push button.
6. GPS continuously updates the user's location.
7. The ESP32 hosts a web dashboard displaying live information.
8. Medicine reminders are generated at regular intervals.

## Web Dashboard

The dashboard displays:

- Latitude
- Longitude
- Fall Detection Status
- Buzzer Status
- Medicine Reminder
- GPS Information

The dashboard refreshes automatically to display the latest sensor data.

## Project Structure

```
Elderly-Care-Monitoring-System/
│
├── code/
│   └── elderly_care_monitoring.ino
│
├── images/
│   ├── dashboard.png
│   ├── flowchart.png
│   └── circuit.jpg
│
├── docs/
│   └── Project_Report.pdf
│
├── README.md
└── LICENSE
```

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Elderly-Care-Monitoring-System.git
```

Open the project in Arduino IDE.

Install the required libraries:

- TinyGPS++
- Adafruit MPU6050
- Adafruit Sensor

Select the ESP32 board.

Update your Wi-Fi credentials in the source code.

Upload the code to the ESP32.

Open the Serial Monitor to obtain the ESP32 IP address.

Enter the IP address into a web browser to access the dashboard.

## Results

The system successfully detects falls, tracks GPS location, activates emergency alerts, and displays real-time information on a web dashboard. It provides reliable monitoring and improves the safety of elderly individuals. :contentReference[oaicite:1]{index=1}

## Future Improvements

- Cloud database integration
- Mobile application
- SMS and email notifications
- Heart rate and SpO₂ monitoring
- AI-based fall prediction
- Firebase support
- Health analytics dashboard

## Authors

T. Manoj Kumar Reddy

Sk. Adil Suhan

Department of Electronics and Communication Engineering

SRM University-AP

## License

This project is intended for educational and research purposes.
