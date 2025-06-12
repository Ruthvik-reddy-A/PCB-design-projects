# 🔧 PCB Design Projects

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Tools](https://img.shields.io/badge/Tools-KiCad-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen/Status-Ongoing-orange)
![Projects](https://img.shields.io/badge/Projects-5-blue)

This combined repository contains self-contained folders for each individual project, along with complete schematics, PCB layouts, documentation, and source files where applicable. It serves both as a personal portfolio and an open-source contribution to the maker and engineering community.

---

## 📁 Projects Overview

### 1. [📦 Breadboard Power Supply](./Breadboard-Power-Supply)

A compact, dual-voltage regulated power supply designed to power breadboard circuits. Ideal for prototyping and educational use.

**Key Features:**
- Outputs: 3.3V and 5V regulated
- Power input via USB or 9V barrel jack
- On/off toggle switches and status LEDs

![Breadboard Power Supply Preview](https://raw.githubusercontent.com/Ruthvik-reddy-A/PCB--BB-PowerSupply/main/images/breadboard-preview.png)

---

### 2. [📦 MCU Datalogger with Built-in 512K EEPROM](./MCU-Datalogger-With-Built-In-512K-EEPROM)

A microcontroller-based data logger that logs sensor or serial data to a 512KB external EEPROM.

**Key Features:**
- ATmega328P-based MCU
- I²C EEPROM (24LC512)
- Power supply filtering and decoupling
- Compatible with UART, I²C sensors or serial interfaces

![MCU Datalogger Preview](https://github.com/user-attachments/assets/a3be4ded-9055-4b7a-9af2-43a87650450a)

---

### 3. [📦 Tiny Solar Power Supply](./Tiny-Solar-Power-Supply)

A miniature solar energy harvesting module capable of charging a Li-ion battery and regulating output to power IoT devices or small loads.

**Key Features:**
- Solar input with MPPT (if supported by controller)
- Li-ion battery charging via TP4056
- Regulated 3.3V/5V output
- Compact PCB layout

![Tiny Solar Supply Preview](https://raw.githubusercontent.com/Ruthvik-reddy-A/PCB--Tiny-Solar-Power-Supply/main/images/solar-preview.png)

---

## 📦 Folder Structure

PCB-design-projects/
├── Breadboard-Power-Supply/
├── MCU-Datalogger-With-Built-In-512K-EEPROM/
└── Tiny-Solar-Power-Supply/


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
