# 🔧 PCB Design Projects

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Tools](https://img.shields.io/badge/Tools-KiCad-green)
![Projects](https://img.shields.io/badge/Projects-5-blue)
![Completed](https://img.shields.io/badge/Completed-5-brightgreen)
![In%20Progress](https://img.shields.io/badge/In_Progress-0-orange)


This combined repository contains self-contained folders for each individual project, along with complete schematics, PCB layouts, documentation, and source files where applicable. It serves both as a personal portfolio and an open-source contribution to the maker and engineering community.

---

## 📁 Projects Overview

### 1. [📦 Breadboard Power Supply](./Breadboard-Power-Supply)

A compact, dual-voltage regulated power supply designed to power breadboard circuits. Ideal for prototyping and educational use.

**Key Features:**
- Outputs: 3.3V and 5V regulated
- Power input via USB or 9V barrel jack
- On/off toggle switches and status LEDs

![Breadboard Power Supply Preview](https://github.com/user-attachments/assets/b80c0f37-1c90-4724-9982-0ad3598e7896)


---

### 2. [📦 MCU Datalogger with Built-in 512K EEPROM](./MCU-Datalogger-With-Built-In-512K-EEPROM)

A microcontroller-based data logger that logs sensor or serial data to a 512KB external EEPROM.

**Key Features:**
- ATmega328P-based MCU
- I²C EEPROM (24LC512)
- Power supply filtering and decoupling
- Compatible with UART, I²C sensors or serial interfaces

![MCU Datalogger Preview](https://github.com/user-attachments/assets/d0e1fe85-adf4-46f1-b762-b7ab736d0cbc)


---

### 3. [📦 Tiny Solar Power Supply](./Tiny-Solar-Power-Supply)

A miniature solar energy harvesting module capable of charging a Li-ion battery and regulating output to power IoT devices or small loads.

**Key Features:**
- Solar input with MPPT (if supported by controller)
- Li-ion battery charging via TP4056
- Regulated 3.3V/5V output
- Compact PCB layout

![Tiny Solar Supply Preview](https://github.com/user-attachments/assets/a0683dc4-0e03-41be-add1-3364a4481c40)

---

### 4. [📦 LED Torch](./LED%20Torch)  
A compact, battery-powered LED torch circuit using minimal components. Designed for efficiency, simplicity, and portability, this project is ideal for learning basic electronics or building a low-cost flashlight.

![image](https://github.com/user-attachments/assets/2b9c05c0-b222-46b4-b012-f38b91d6988f)

---

### 5. [📡 GPS + GSM Tracker with EEPROM Logging](https://github.com/Ruthvik-reddy-A/PCB-design-projects/tree/main/GPS%20%2B%20GSM%20Tracker%20with%20EEPROM%20Logging)
A compact, ESP32-S3-based IoT tracker that logs GPS data locally and transmits position via GSM. Ideal for asset tracking, vehicle monitoring, and offline location logging in remote or mobile environments.

**Key Features:**
- Microcontroller: ESP32-S3-WROOM-1 with Wi-Fi + BLE
- GPS Module: NEO-8Q for real-time latitude/longitude tracking
- GSM Module: SIM800C for SMS or GPRS-based data transmission
- EEPROM: I²C-based 24LC256 for offline GPS data logging

**Power Supply:**
- Input: 3.7V LiPo battery
- Charging: TP4056 module with battery protection
- Regulation: AMS1117-3.3 for ESP32, Boost converter for SIM800C

**Communication:**
- 3× UARTs for GPS, GSM, and FTDI debugging
- 1× I²C for EEPROM and future expansion
- SPI pins available for SD card or display

**Indicators:**
- LED status for power, charging, and ESP32 boot
- Power control switch for full system on/off

![image](https://github.com/user-attachments/assets/5bcc69d6-d367-4f33-bdab-899ec2e042b4)



---

## 📦 Folder Structure

Each folder includes:
- ✅ `README.md`
- ✅ `.gitignore`
- ✅ Schematics, PCB Layouts
- ✅ Bill of Materials (BOM)
- ✅ Gerber & Drill files
- ✅ Source code (if applicable)

---

## 🙌 Contributions

Feel free to fork or suggest improvements. Each project is self-contained and documented to allow easy reuse or remixing.

---

## 🔗 Related Repositories (Now Archived/Private)

These projects were originally developed in individual repositories:
- `PCB--BB-PowerSupply`
- `PCB--MCU-Datalogger`
- `PCB--Tiny-Solar-Power-Supply`

They have been combined here for easier access and long-term maintenance.
