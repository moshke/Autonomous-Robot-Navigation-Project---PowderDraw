# PowderDraw – Autonomous Drawing Robot

## 📌 Overview
PowderDraw is an autonomous mobile robot designed to draw large-scale patterns using colored powder. Developed as a final-year engineering project, it combines precise localization, real-time control, and sensor fusion to enable fully autonomous operation over open areas.

The robot utilizes the **Pixhawk** flight controller running **ArduPilot**, along with a **Raspberry Pi 4** for communication and control logic.
It integrates GPS, IMU, optical flow, and wheel encoders, using an **Extended Kalman Filter (EKF)** for accurate localization and navigation.

## 🎯 Project Goals
- Design a low-cost, scalable robot for surface design using powder.
- Implement accurate autonomous navigation over a 30x30 meter field.
- Build a modular control architecture using open-source tools.
- Create a reliable powder-dispersion system controlled in real time.

---

## 🧠 Key Features
- **Sensor Fusion** using EKF with GPS, IMU, Optical Flow, and wheel encoders.
- **Navigation & Control** via ArduPilot and Mission Planner, with customized PID tuning.
- **Custom Powder Dispersion System** using a solenoid valve and servo, activated based on robot position.
- **Real-time Wireless Communication** using Wi-Fi and MAVLink between Raspberry Pi and Pixhawk.
- **Algorithmic Enhancements**: Lucas-Kanade Optical Flow, EKF parameter tuning, and real-time failsafe modifications.

---

## 🛠️ Hardware Components
- Pixhawk 2.4.8 Flight Controller
- Raspberry Pi 4
- Hall Effect Encoders
- GPS Module (Ublox M8N)
- MPU6000 IMU + Magnetometer
- LIDAR (optional integration for future expansion)
- Optical Flow Camera
- Servo-Controlled Powder Valve
- Brushed DC Motors with Motor Drivers
- Custom 3D-printed chassis & mechanical mounts
- 12V battery pack (LiPo) for motor and logic power

---

## 🧰 Software Architecture
- **Firmware**: ArduPilot custom-tuned for ground vehicles
- **Communication**: MAVLink between Raspberry Pi & Pixhawk
- **Ground Control**: Mission Planner (Route planning + live telemetry)
- **Algorithms**:
  - EKF (sensor fusion)
  - PID control tuning
  - Optical Flow via Lucas-Kanade
  - Powder activation based on waypoints
- **Languages**: C++, Python

- ## 📽️ Video Demo
👉 [Watch the project in action on YouTube](https://youtu.be/O9t15PjKslc)

---


