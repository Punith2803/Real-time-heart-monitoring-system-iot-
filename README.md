# Real-time-heart-monitoring-system-iot-

Real-Time Heart Rate Monitoring System Using IoT (ESP8266 + MAX30102 + Blynk)

This repository contains the code and documentation for a real-time heart-rate and SpO2 monitoring system built using an ESP8266 Wi‑Fi microcontroller, a MAX30102 pulse oximeter sensor, and the Blynk mobile app. The project continuously measures heart rate and oxygen saturation, sends the processed data over Wi‑Fi to the Blynk cloud, and displays it on a smartphone dashboard with configurable alert thresholds for abnormal values.​

Main features:

Continuous acquisition of heart-rate and SpO2 data from the MAX30102 sensor and on-board processing using the ESP8266.​

Real-time data transmission to the Blynk server and visualization on the Blynk mobile app, including virtual pins for live graphs and numeric widgets.​

Threshold-based notifications from the Blynk app if the heart rate goes outside the configured safe range (e.g., via events/logs/notifications).​

Hardware:

ESP8266 development board (3.3 V supply)

MAX30102 pulse oximeter and heart-rate sensor

Jumper wires and a stable 3.3 V power supply

Android/iOS smartphone with the Blynk app installed​

Getting started:

Open the Arduino IDE, install the required libraries (ESP8266 WiFi, Blynk, Wire, MAX30102/DFRobot MAX30102), and update the auth token and Wi‑Fi credentials in the sketch.​

Wire MAX30102 to ESP8266 over I2C (SDA → GPIO4/D2, SCL → GPIO5/D1, VCC → 3.3 V, GND → GND), flash the firmware, and configure the corresponding widgets in the Blynk template to read from the defined virtual pins.​

Place a finger properly on the sensor and open the Blynk app to view live heart-rate and SpO2 values, along with alerts when configured thresholds are crossed.​

Use this project as a starting point for low-cost IoT health monitoring, and extend it with additional metrics, better filtering, or cloud integrations as needed.​
