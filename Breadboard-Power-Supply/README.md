# ⚡ Breadboard Power Supply

A compact, dual-voltage regulated power supply module designed specifically to power circuits on a breadboard. This project provides reliable 3.3V and 5V outputs and is ideal for prototyping and electronics education.

---

## 📸 Preview

![Breadboard Power Supply Preview](images/breadboard-preview.png) <!-- Replace with actual image if available -->

---

## ⚙️ Features

- ✅ Provides both **3.3V** and **5V** outputs
- 🔌 Accepts input from USB or DC barrel jack (6V–12V)
- 🧰 Onboard voltage regulators (e.g., AMS1117)
- 📎 Designed to plug directly into standard breadboards
- 🔋 On/Off toggle switches for each rail
- 🧲 Polarity protection and status LEDs included

---

## 🔧 Circuit Overview

This power module uses two linear regulators (AMS1117 or similar) to deliver stable voltages for breadboard circuits. It includes onboard:

- Input power jack (DC barrel or USB micro-B)
- Two low-dropout regulators: one for 3.3V, one for 5V
- Slide switches for enabling/disabling each voltage rail
- Pin headers to mount directly on a breadboard
- Power indicator LEDs

---

## 📋 Bill of Materials (BOM)

| Component | Value / Part       | Description                         |
|-----------|--------------------|-------------------------------------|
| U1        | AMS1117-5.0        | 5V Linear Regulator                 |
| U2        | AMS1117-3.3        | 3.3V Linear Regulator               |
| D1        | 1N4007             | Input polarity protection diode     |
| C1, C2    | 10µF Electrolytic  | Input/output filter capacitors      |
| R1, R2    | 330Ω               | LED current-limiting resistors      |
| LED1, LED2| Red/Green LEDs     | Power indicators                    |
| SW1, SW2  | SPDT Slide Switch  | ON/OFF control for 5V/3.3V rails     |
| J1        | DC Barrel Jack     | Power input                         |
| J2        | USB (optional)     | Alternate power input               |
| Header    | Male Pin Header    | Breadboard pins                     |

---

## 🛠️ Assembly & Usage

1. **Solder all components** as per the PCB layout.
2. Insert the module into a breadboard.
3. Connect 6–12V input via USB or barrel jack.
4. Use the toggle switches to activate 5V or 3.3V output rails.
5. Verify voltages with a multimeter before connecting sensitive components.

---

## 📦 Folder Structure

