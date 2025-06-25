# 📡 IoT GPS-GSM Tracker with ESP32-S3 + EEPROM Logging

An ESP32-S3 based IoT hardware project for **location tracking** using a **GPS module (NEO-8Q)**, with real-time updates via **GSM (SIM800C)** and local data logging using an **I²C EEPROM (AT24C256)**. Power is managed via a **3.7V LiPo battery**, **TP4056 charger**, and **MT3608 boost converter**.

---

## 🧩 Features

- 📍 Real-time GPS tracking (NEO-8Q)
- 📡 GSM-based data transmission (SIM800C)
- 📦 EEPROM logging (AT24C256) for offline storage
- 🔋 Battery-powered with charging via TP4056
- ⚡ Boost conversion to 4.1V using MT3608
- 🧠 Controlled by ESP32-S3 (WROOM-1)

---

## 🔋 Power Architecture

| Source         | Voltage | Connected To     |
|----------------|---------|------------------|
| 3.7V LiPo      | 3.0–4.2V | TP4056 + MT3608  |
| TP4056 OUT     | 3.7V     | MT3608 Input     |
| MT3608 OUT     | 4.1V     | SIM800C VBAT     |
| LDO Regulator  | 3.3V     | ESP32, EEPROM, GPS |

---

## 🔌 Module Connections

### ESP32-S3 ↔ GPS (NEO-8Q)
| ESP32 Pin | GPS Pin |
|-----------|---------|
| RX2       | TX      |
| TX2       | RX      |
| 3.3V      | VCC     |
| GND       | GND     |

### ESP32-S3 ↔ SIM800C (via TXS0108E level shifter)
| ESP32 Pin | SIM800C Pin |
|-----------|-------------|
| TX1       | RX          |
| RX1       | TX          |
| GND       | GND         |
| OE (TXS)  | 3.3V        |

### ESP32-S3 ↔ EEPROM (AT24C256)
| ESP32 Pin | EEPROM Pin |
|-----------|-------------|
| GPIO21    | SDA         |
| GPIO22    | SCL         |
| 3.3V      | VCC         |
| GND       | GND         |

---

## 📐 Schematic Overview

📎 The following components are included:
- ESP32-S3-WROOM-1
- NEO-8Q GPS module (passive antenna)
- SIM800C GSM module with SMA antenna
- MT3608 boost converter
- TP4056 LiPo charger module
- AT24C256 EEPROM (I²C)
- Status LEDs and EN/BOOT buttons

📷 *![image](https://github.com/user-attachments/assets/753b703e-012b-43aa-bc9f-b1255291e6f5)*

![image](https://github.com/user-attachments/assets/4f7b27f5-4cd9-4600-90d7-56db0fc6dff9)


---



