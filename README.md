# PROTOX Automatic Floor Cleaning Robot

An ESP32-based automatic floor cleaning robot with obstacle avoidance, 
water spraying, voice announcements and WiFi phone control.

> 📌 **Repository status:** README published. The firmware (`protox_main/protox_main.ino`) and wiring notes (`docs/wiring.md`) have not been added to this repository yet.

## Features
- Automatic movement and obstacle avoidance
- Auto water spray every 10 seconds
- Voice announcement on obstacle detection (ISD1820)
- Phone control via WiFi webpage
- Manual and Auto modes
- Emergency stop

## Hardware
- ESP32
- L298N Motor Driver
- 2x Geared DC Motors
- HC-SR04 Ultrasonic Sensor
- 5V Relay Module + BC547
- DC Submersible Pump
- ISD1820 Voice Module
- LM2596 Buck Converter
- 3S 18650 Battery (11.1V)

## Pin Mapping
| Component | ESP32 Pin |
|---|---|
| ENA | GPIO 25 |
| IN1 | GPIO 26 |
| IN2 | GPIO 27 |
| ENB | GPIO 33 |
| IN3 | GPIO 14 |
| IN4 | GPIO 19 |
| TRIG | GPIO 5 |
| ECHO | GPIO 18 |
| PUMP | GPIO 2 |
| VOICE | GPIO 21 |

## WiFi Control
- Network: PROTOX
- Password: 12345678
- Open: http://192.168.1.1

## How to Use
1. Upload code to ESP32
2. Remove USB
3. Turn ON main switch
4. Connect phone to PROTOX wifi
5. Open http://192.168.1.1
6. Control robot from phone

## Built By
PROTOX Engineering Team
