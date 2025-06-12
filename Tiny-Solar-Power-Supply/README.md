# 🔆 Tiny Solar Power Supply
> Sunlight In, 3.3V Out — A Miniature Solar-Charged Boost Converter

This project is a **solar-powered boost converter** that takes input from a small solar panel charging a 1.2V NiMH battery and steps it up to a **regulated 3.3V** output. It’s ideal for powering microcontrollers or low-power circuits from solar-charged AA(A) batteries.

---

## 📸 Preview

![PCB Preview](![image] https://github.com/user-attachments/assets/955f0023-5773-45fc-b709-64f48a1f761e) 

---

## ⚙️ Features

- ✅ Converts 1.2V battery to **stable 3.3V output**
- ☀️ Automatically **shuts down** while solar panel is charging
- 🔋 Uses **NiMH AA(A)** battery and simple solar panel
- 🔧 Optional **manual On/Off** control jumper
- 📏 Compact PCB fits inside reused garden light enclosures

---

## 🔧 Technical Overview

- **IC**: AP3015 (Micropower Step-Up Converter)
- **Input Voltage**: 1V–1.2V (NiMH AA battery)
- **Output Voltage**: ~3.3V (set via resistor divider)
- **Max Output Current**: 100–350 mA depending on version
- **Control Logic**: Automatic shutdown via MOSFET on solar detect
- **Applications**: Low-power MCUs, LED drivers, outdoor sensors

---

## 🖥️ Circuit Diagram

The boost converter is built around the **AP3015A** DC-DC converter and includes standard passive filtering (L1, C1–C3) and voltage divider resistors (R1/R2) to regulate the output to ~3.3V.

![Circuit Diagram](![image](https://github.com/user-attachments/assets/77fa3d0c-b3b5-4790-b374-ec5240d4246e)


> Output voltage is defined by:  
> `VOUT = 1.23 × (1 + R1/R2)` → Gives ~3.3V with R1 = 1MΩ, R2 = 604kΩ

---

## 📋 Bill of Materials (BOM)

| Component | Value           | Package    |
|----------:|------------------|------------|
| IC1       | AP3015 / AP3015A | SOT-23-5   |
| L1        | 10 µH, 680 mA     | Resistor-style |
| D1, D2    | SS14             | DO-214AC   |
| T1        | 2N7002           | SOT-23     |
| R1, R4    | 1 MΩ             | 0805       |
| R2        | 604 kΩ, 1%       | 0805       |
| R3        | 10 kΩ            | 0805       |
| C1        | 4.7 µF, 50V X7R  | 0805       |
| C2        | 22 µF, 10V X7R   | 1206       |
| C3        | 10 pF, 50V X7R   | 0805       |
| K1–K4     | Pin headers (2-pin, 2.54 mm / 2.00 mm) | — |

---

## 🪛 PCB Design

The PCB is designed to be compact enough to fit in standard garden light enclosures. It features:

- Pin headers for solar input, battery, output, and shutdown control
- Through-hole and SMD components
- Single-layer layout (optional)

> 📁 PCB files available in this repo: `schematics/`, `gerbers/`, and `layouts/`

---

## 🔗 Resources

- 📄 [Original Article](https://elektormagazine.com/labs/tiny-solar-supply)
- 📦 [Elektor BOM Reference](https://elektor.com)
- 🔌 [Seeed Studio Solar Panel](https://elektor.com/19131)
- 🔍 [AP3015 Datasheet](https://www.diodes.com/assets/Datasheets/AP3015.pdf)

---

## 🧪 Usage Notes

- Ensure your solar panel can supply >1.5V under sunlight
- Use a rechargeable NiMH AA cell (1.2V typical)
- T1 (2N7002) can be left out if you don’t want auto shutoff
- Test the voltage at the output header before connecting sensitive electronics

---

## 🙋‍♂️ Author & Credits

Originally designed and documented by **Clemens Valens** for Elektor Labs  
Adapted and implemented by **Ruthvik Reddy A** as part of personal PCB project collection.

Questions or feedback? Email: `reddy.ruthvik0411@gmail.com`

