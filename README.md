# Edge–Fog–Cloud IoT Architecture using ESP32, Raspberry Pi, and Django

An IoT-based embedded system implementing the **Edge–Fog–Cloud architecture** using an ESP32, Raspberry Pi, Flask, WebSocket, and Django. The system performs real-time environmental monitoring with a DHT22 sensor and automatically controls an LED based on temperature thresholds.

---

## Objectives

- Design an embedded system for a real-world IoT application.
- Implement an Edge–Fog–Cloud architecture.
- Enable real-time communication using WebSockets.
- Develop an automated temperature-based control system.
- Integrate embedded devices with cloud services.

---

## System Architecture

```
                    +----------------------+
                    |     Cloud Layer      |
                    | Django Web Server    |
                    | Data Storage         |
                    | Visualization        |
                    +----------▲-----------+
                               |
                          REST API
                               |
                    +----------▼-----------+
                    |      Fog Layer       |
                    | Raspberry Pi         |
                    | Flask Server         |
                    | WebSocket Server     |
                    | Decision Making      |
                    +----------▲-----------+
                               |
                        WebSocket
                               |
                    +----------▼-----------+
                    |     Edge Layer       |
                    | ESP32 Development    |
                    | DHT22 Sensor         |
                    | LED Control          |
                    +----------------------+
```

---

## Hardware Components

- ESP32 Development Board
- DHT22 Temperature & Humidity Sensor
- LED
- Wi-Fi Router
- Raspberry Pi
- Micro USB Cable

---

## Software

- Arduino IDE
- Python 3
- Flask
- WebSocket
- Django
- Raspberry Pi OS
- Visual Studio Code

---

## Project Features

- Real-time temperature and humidity monitoring
- WebSocket communication
- Flask Web Server
- Edge–Fog–Cloud architecture
- Automatic LED control
- REST API integration
- Cloud-ready architecture

---

## Tasks Completed

### Task 01 – WebSocket Communication

- Connected ESP32 with Raspberry Pi
- Read DHT22 sensor data
- Sent JSON data using WebSocket
- Verified real-time communication

---

### Task 02 – Flask + WebSocket Integration

- Developed Flask server
- Integrated WebSocket server
- Used multithreading for concurrent execution
- Displayed sensor data in real time

---

### Task 03 – Automatic Temperature Control

- Compared temperature against a threshold
- Sent ON/OFF commands to ESP32
- Automatically controlled LED
- Prepared data for Django cloud integration

---

## Communication Flow

```
DHT22 Sensor
      │
      ▼
ESP32
      │
WebSocket
      │
      ▼
Raspberry Pi
(Flask + WebSocket)
      │
Decision Making
      │
 ┌────┴────┐
 │         │
 ▼         ▼
LED      Django Server
Control   (Cloud)
```

---

## Repository Structure

```
Embedded-System-Lab/
│
├── ESP32/
│   ├── websocket_client.ino
│   └── libraries
│
├── RaspberryPi/
│   ├── websocket_server.py
│   ├── flask_server.py
│   └── requirements.txt
│
├── Django/
│
├── Images/
│
└── README.md
```

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Embedded System Design
- IoT System Development
- Edge–Fog–Cloud Computing
- ESP32 Programming
- Raspberry Pi Programming
- Flask Web Framework
- WebSocket Communication
- REST APIs
- Sensor Integration
- Automatic Device Control
- Distributed IoT Architecture

---

## Technologies Used

- C++
- Python
- Arduino IDE
- Flask
- Django
- WebSocket
- ESP32
- Raspberry Pi
- IoT

---

## Future Improvements

- MQTT integration
- Database storage
- Interactive dashboard
- Mobile application
- Multiple sensor nodes
- Cloud analytics
- User authentication

---

## Author

**Thisara Siriwardhana**

Computer Engineering Undergraduate

---

## License

This project was developed for educational and learning purposes.
