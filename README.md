# Smart Water Level Monitoring & Automatic Pump Control System

Real-time water level monitoring system with automatic pump control and IoT remote monitoring.

![Project Photo](photo.jpg)

## Features
- Ultrasonic water level sensing (HC-SR04) with 5-sample averaging for ±1cm accuracy
- Automatic 12V pump control via relay module
- OLED display (SSD1306, I2C) showing live water level, distance, and pump status
- Buzzer alerts for tank full and critically low conditions
- Remote IoT monitoring via Blynk smartphone app through ESP32 WiFi bridge

## Hardware
- STM32 Nucleo-F401RE (main controller)
- ESP32 DevKit (WiFi/IoT bridge)
- HC-SR04 ultrasonic sensor
- SSD1306 128x32 OLED display (I2C)
- SRD-12VDC relay module
- 12V DC submersible water pump
- Piezo buzzer

## Software
- **STM32 firmware:** C/C++ on ARM Mbed (Keil Studio Cloud)
- **ESP32 firmware:** Arduino IDE with Blynk library

## Communication Protocols
- I2C (OLED display)
- UART (STM32 ↔ ESP32 data bridge)
- HTTP/WiFi (ESP32 → Blynk cloud)

## File Structure
- `stm32_main/main.cpp` — STM32 Nucleo firmware
- `esp32_blynk/esp32_blynk_bridge.ino` — ESP32 Blynk bridge firmware

## Course
EFB 2073 – Microprocessors & Computer Architecture
Universiti Teknologi PETRONAS | January 2026 Semester
