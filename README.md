# Light-Tracking-Launcher

Light-Tracking-Launcher is an Arduino-based system that uses LDR sensors and servo motors to track a light source. It applies a closed-loop control algorithm for real-time alignment and supports serial/Bluetooth commands, EEPROM calibration, and an optional launcher mechanism triggered when alignment conditions are met.

---

## Features

- 4 LDR sensors for light direction detection  
- Pan/tilt servo control system  
- Closed-loop tracking control  
- Serial and Bluetooth command interface  
- EEPROM-based calibration storage  
- Optional mechanical launcher trigger  

---

## Hardware

- Arduino UNO / Nano / Mega  
- 4x LDR sensors  
- 3x servo motors (pan, tilt, launcher)  
- Bluetooth module (HC-05 / HC-06)  
- Laser or light source (optional for testing)  
- Voltage divider for battery monitoring  

---

## Commands

- `help()` → Show available commands  
- `track(0/1)` → Enable/disable tracking  
- `lat(angle)` → Set tilt angle  
- `lon(value)` → Set pan position  
- `fire()` → Activate launcher  
- `laser(0/1)` → Control laser  
- `battery()` → Show battery voltage  

---

## Calibration

Sensor calibration values are stored in EEPROM to improve accuracy across different lighting conditions.

---

## Notes

- Ensure stable power supply for servos  
- Bluetooth and USB serial can be used interchangeably  
- Tracking should be enabled only after proper calibration  
