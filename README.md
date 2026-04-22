**Environmental Sensor Firmware (ESP32)**
Overview

This project is an ESP32 based environmental monitoring system that reads and processes data from multiple sensors to measure air, water, and soil conditions.

Features
Air Temperature monitoring
Humidity measurement
pH sensing
TDS measurement (manual potentiometer method)
Liquid temperature monitoring
Soil moisture detection
Real time serial output
Basic filtering and stable readings
Hardware Used
ESP32 MCU
Temperature and Humidity Sensor
pH Sensor Module
TDS Sensor Module
Water Temperature Sensor
Soil Moisture Sensor
Working Principle

The firmware initializes all sensors, reads raw data from analog and digital inputs, processes the values using filtering and calibration, and outputs stable readings via serial communication for monitoring.

Pin Configuration (Example)
Sensor	ESP32 Pin
pH Sensor	GPIO36
TDS Sensor	GPIO39
Sensor Enable	GPIO19
Others	As per configuration
Getting Started
1. Upload Firmware
Open code in Arduino IDE or PlatformIO
Select ESP32 board
Upload to device
2. Open Serial Monitor
Set baud rate (e.g., 115200)
Observe sensor values
Testing
Verify each sensor individually
Compare readings with reference instruments
Perform stability test for 60 seconds
Calibrate pH and TDS for accuracy
Calibration
pH: Use standard buffer solutions (pH 4 and pH 7)
TDS: Use known ppm solution or voltage reference
Temperature: Compare with standard thermometer
Output Example
Temp: 28.5°C | Humidity: 65%
pH: 7.02
TDS: 120 ppm
Water Temp: 29.1°C
Soil Moisture: 75%
Applications
Environmental monitoring
Agriculture and soil analysis
Water quality testing
IoT based sensing systems
Notes
Ensure proper grounding for analog sensors
Allow settling time for pH and TDS sensors
Use stable power supply for accurate readings
License

This project is open source and free to use for development and educational purposes.
