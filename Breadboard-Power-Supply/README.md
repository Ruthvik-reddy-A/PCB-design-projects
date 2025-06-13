# Breadboard Power Supply Module

This repository documents a simple yet essential module for electronics prototyping: the Breadboard Power Supply. It provides a regulated voltage output (3.3V and/or 5V) directly to your breadboard, making it ideal for microcontroller projects, sensor interfacing, and other DIY circuits.

## ⚙️ Features.
* Input voltage: 6V–12V DC via barrel jack or 5V USB
* Output voltage: Selectable 3.3V / 5V via jumper or switch
* Current capacity: Up to 500mA–1A (depends on regulator used)
* On/Off power switch
* Fits standard breadboard power rails
* Power indicator LED

---

## 🔧Schematic
![image](https://github.com/user-attachments/assets/b7b1bc69-9700-4db6-8d01-e2a787455f88)



## 🖼️ PCB Preview
Top View of the PCB:

![image](https://github.com/user-attachments/assets/661a7166-1eba-4359-a028-bf145ea16efa)



Back View (if applicable):

![image](https://github.com/user-attachments/assets/43be32aa-a716-456f-9530-5f55e0f8d56b)


---

## 🧩 Components Used
| Component         | Description                            |
| ----------------- | -------------------------------------- |
| Voltage Regulator | AMS1117 / LM317 / 7805                 |
| Capacitors        | For filtering and stability            |
| Barrel Jack / USB | For external power input               |
| Slide Switch      | To turn power on/off                   |
| Jumper Pins       | Voltage selector (3.3V / 5V)           |
| Header Pins       | To connect with breadboard power rails |

## 🔌 How It Works
1. Supply DC power (6–12V) via the barrel jack or connect 5V via USB.
2. The onboard voltage regulator converts this input to a stable 5V or 3.3V.
3. The output is routed to the breadboard power rails via header pins.
4. Use jumper caps to select the voltage output (if applicable).

## ⚠️ Notes
* Always check input voltage range to prevent regulator damage.
* Verify polarity before connecting to your breadboard.
* Do not exceed the current capacity of the regulator.

## 🖼️ Circuit Diagram

> (Include a circuit schematic or image here if available)

## 🧪 Applications
* Powering Arduino, ESP32, STM32, and other MCUs
* Sensor testing and interfacing


