# 🧾 MCU Data Logger – PCB Design

This repository contains the complete PCB design files and documentation for a microcontroller-based data logger with 512KB external EEPROM. The system is designed to log sensor data and store it in non-volatile memory, making it ideal for long-term, standalone data acquisition applications.

---

🔧 Designed using: KiCad 

📐 PCB Type: 2-layer, through-hole/SMD hybrid

---

## 🔋 Key Features
* Microcontroller-based core (ATmega328P / STM32 / ESP32)
* 512KB I²C EEPROM (e.g., 24LC512) for data storage
* Optional RTC (DS3231) for timestamped logging
* UART/USB interface for data extraction
* Breadboard-compatible or standalone PCB footprint
* Power input: USB / 5V header / Li-Ion with LDO
---


## 🔧 Hardware Block Diagram
![image](https://github.com/user-attachments/assets/c6f2ce94-99b2-4912-8d6f-8fb5d41b08d6)


## 🖼️ PCB Preview
Top View of the PCB:

![Front View](https://github.com/user-attachments/assets/e1956d6c-d059-417f-8eb1-6aa06948d26c)



Back View (if applicable):

![Back View](https://github.com/user-attachments/assets/a21a89dd-ddf9-4ecb-bde0-6d50f5a780ab)


---

## 📐 Pinouts & Interfaces

| Interface | Purpose               | Pin(s)            |
| --------- | --------------------- | ----------------- |
| I²C       | EEPROM, RTC           | SDA, SCL          |
| UART      | Serial communication  | TX, RX            |
| Power     | +5V / GND / Battery   | VIN, GND          |
| Sensor    | Analog/Digital inputs | A0, A1, D2, D3... |

---

## 📥 Data Logging Behavior
* Data sampled every X seconds
* Stored in EEPROM in binary or CSV-friendly format
* Memory managed using circular buffer logic
* Data dump via UART/USB when connected to host

---

## 🛠️ Fabrication & Assembly
* Use the included Gerber files (/gerbers) for fabrication
* Reference BOM (/bom.csv) for components
* Optionally reflow or hand-solder depending on design

---
