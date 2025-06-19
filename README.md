# 🚗 Obstacles Avoiding Race

An Arduino-based autonomous obstacle avoiding robot project, developed as part of the Smart System Design course at SR University. The robot is designed to intelligently detect and avoid obstacles using ultrasonic sensors and servo motor coordination.

## 🔧 Project Overview

This project aims to build a self-navigating robot that can:
- Detect obstacles using ultrasonic sensors
- Decide optimal direction using servo motor rotation
- Control movement with L293D motor driver
- Be operated via Bluetooth (HC-05) and voice commands

## 🧠 Features

- Autonomous obstacle avoidance using ultrasonic distance sensing
- Bluetooth control via HC-05 module
- Voice command integration for robot control
- Arduino UNO-based control with real-time decision making
- Built-in safety alerts using buzzer and lights

## 🖼️ Block Diagram

The system integrates:
- Ultrasonic sensor (HC-SR04)
- Servo motor for directional scanning
- Arduino UNO microcontroller
- L293D Motor Driver for motor control
- HC-05 Bluetooth module

## 🔌 Hardware Components

| Component             | Description                          |
|----------------------|--------------------------------------|
| Arduino UNO          | Main microcontroller                 |
| Ultrasonic Sensor    | Distance measurement and obstacle detection |
| Servo Motor          | Controls sensor rotation direction   |
| L293D Motor Driver   | Drives motors                        |
| HC-05 Bluetooth      | Enables wireless control             |
| DC Motors (x4)       | Drives the robot wheels              |
| Power Source         | Battery (7-12V)                      |

## 💻 Software

- **Arduino IDE** for writing and uploading code
- **C++** for programming robot logic
- **Bluetooth serial monitor** (e.g. Android app or terminal emulator)

## 🧾 How It Works

1. Robot moves forward by default.
2. When an obstacle is detected:
   - It stops and scans left/right using servo motor
   - Based on sensor data, it turns in the direction with more clearance
3. Commands can also be sent via:
   - Bluetooth ("F", "B", "L", "R", "S")
   - Voice control (custom signals like '^', '-', '<', etc.)

## 🧠 Sample Commands

| Command | Action       |
|---------|--------------|
| F       | Move Forward |
| B       | Move Backward|
| L       | Turn Left    |
| R       | Turn Right   |
| S       | Stop         |

## 🔮 Future Scope

- Integrating autopilot features for larger scale robotic systems
- Industrial automation and smart vehicle navigation
- Smart cleaning and delivery bots
