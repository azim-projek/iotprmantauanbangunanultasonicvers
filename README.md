# Smart Building Monitor (Ultrasonic + MPU6050)

## Project Overview
The Smart Building Monitor is an IoT-based system designed to monitor the structural stability of a building or object in real-time. It uses an ultrasonic sensor to measure distance and an MPU6050 accelerometer/gyroscope to detect tilt. Alerts are sent via Telegram and a buzzer when abnormal conditions are detected.

---

## Features
- **Distance Monitoring:** Measures distance from the sensor to the object using an ultrasonic sensor (HC-SR04).
- **Tilt Detection:** Measures tilt angle using MPU6050.  
- **Alerts:**  
  - Normal: No alert  
  - Warning: Slow buzzer, Telegram warning message  
  - Critical: Fast buzzer, Telegram critical message  
- **WiFi + Telegram Bot Integration:** Sends instant notifications to the user.  
- **Moving Average Filtering:** Smooths sensor readings for stability.

---

## Hardware Components
- **ESP32**: Main controller handling sensors and WiFi.
- **Ultrasonic Sensor (HC-SR04)**: Measures distance to the monitored object.
- **MPU6050**: Accelerometer and gyroscope for tilt measurement.
- **Buzzer**: Provides audible alerts.
- **Power Supply**: ESP32 powered via USB or battery.

---

## Software Components
- **Arduino IDE**
- Libraries:
  - `Wire.h`
  - `MPU6050.h`
  - `WiFi.h`
  - `WiFiClientSecure.h`
  - `UniversalTelegramBot.h`
