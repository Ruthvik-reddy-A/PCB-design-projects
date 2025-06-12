# 🔦 LED Torch Project

A simple, compact, and low-power LED torch circuit designed for basic lighting applications. This project demonstrates the use of common electronic components to build a reliable and reusable LED lighting system powered by batteries.

---

## 📸 Preview

![LED Torch Preview](https://github.com/user-attachments/assets/1f22efac-da1d-4c98-9e61-dfe37c2db39d)
 <!-- Replace with actual path if available -->

---

## 📸 Schematic

![image](https://github.com/user-attachments/assets/2ff32537-69d5-49e4-9009-28fcb989187e)

---

## ⚙️ Features

- ✅ Efficient LED driver using discrete components
- 🔋 Battery-powered (1.5V/3V/AA/AAA or coin cell based)
- 🔄 Optional on/off switch or push button
- 💡 Designed for white LED (or red/green/blue options)
- 🪛 Minimal component count for easy DIY assembly

---

## 🔧 Circuit Overview

This LED torch uses a simple boost converter or current-limiting resistor circuit depending on configuration. It lights up one or more LEDs from a low-voltage battery source, offering basic illumination.

Typical components used:
- Transistor (e.g. 2N2222 / BC547)
- White LED (3.0–3.3V forward voltage)
- Resistor for current control (100–470Ω)
- Power switch or jumper
- Battery holder for AA / AAA or coin cells

---

## 📋 Bill of Materials (BOM)

| Component     | Value / Part       | Description                         |
|---------------|--------------------|-------------------------------------|
| Q1            | 2N2222 / BC547      | NPN transistor                      |
| R1            | 100–470Ω            | LED current-limiting resistor       |
| LED1          | 5mm White LED       | Main torch light                    |
| S1            | SPST Switch / Jumper | Torch On/Off control                |
| Battery       | AA / AAA / Coin cell | Power source (1.5–3V)              |
| PCB           | Custom single-sided | Compact torch layout                |

---

## 🖥️ PCB Design

The PCB is compact and designed to fit inside a small torch enclosure or be mounted on a keychain or clip. It includes pads for the switch, LED, and battery holder.

> PCB layout, schematic, and Gerber files are included in the `/pcb/` folder.

---

## 🚀 Usage Instructions

1. Solder all components as per schematic
2. Insert battery and close the case
3. Toggle the switch to power the LED
4. For higher brightness, use 2 LEDs in parallel and adjust the resistor accordingly

---

## 🧰 Tools Used

- 🖥️ KiCad / EasyEDA (for schematic & PCB)
- 🔧 Soldering iron & basic tools
- 🧪 Multimeter (for circuit verification)

---

## 📄 License

This project is open-source under the [MIT License](../LICENSE).  
Feel free to modify, build upon, or use it in your own projects.

---

## 🙋‍♂️ Author & Credits

Designed by **Ruthvik Reddy A**  
For questions, reach out at: `reddy.ruthvik0411@gmail.com`


