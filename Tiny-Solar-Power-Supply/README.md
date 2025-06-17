# ☀️ Tiny Solar Power Supply

A minimalist, solar-powered **boost converter** circuit that charges a single 1.2V NiMH AA battery and provides a regulated **3.3V output**, ideal for microcontrollers or low-power IoT devices.

Originally published in Elektor Magazine, this design is adapted to fit into small enclosures like salvaged solar garden lights. It balances simplicity, efficiency, and practicality for real-world solar energy harvesting.

---

## 📸 Preview

![Tiny Solar Supply PCB Preview](https://github.com/user-attachments/assets/faf72fd4-a545-4611-99ff-ec73eee9e7c5)
<!-- Replace with actual image path -->

---

## ⚙️ Key Features

- 🔋 Charges a 1.2V NiMH AA cell via small solar panel
- ⚡ Boosts battery voltage to regulated **3.3V output**
- ⛔ Auto-disables output when panel is exposed to light (configurable)
- 🔄 Optional manual On/Off jumper
- 📦 Small, easy-to-assemble PCB — fits inside common garden light enclosures

---

## 🔧 Technical Details

- **Controller IC**: AP3015 (Micropower DC-DC Boost Converter)
- **Input**: 1V–1.2V (NiMH battery)
- **Output**: ~3.3V regulated (via R1/R2 voltage divider)
- **Max Output Current**:  
  - 100 mA with AP3015A  
  - 350 mA with AP3015
- **Battery Charging**: Solar panel through Schottky diode (SS14)
- **Shutdown Logic**: Uses 2N7002 MOSFET to disable output when sunlight is present

---

## 📋 Bill of Materials (BOM)

| Component | Value / Part       | Description                         |
|-----------|--------------------|-------------------------------------|
| IC1       | AP3015 / AP3015A   | Boost Converter IC                  |
| L1        | 10 µH              | Inductor, 680 mA (resistor-style OK)|
| D1, D2    | SS14               | Schottky diodes                     |
| T1        | 2N7002             | MOSFET for shutdown control         |
| R1, R4    | 1 MΩ               | Feedback + gate pull-down resistors |
| R2        | 604 kΩ             | Voltage divider (sets 3.3V)         |
| R3        | 10 kΩ              | Gate resistor                       |
| C1        | 4.7 µF, 50V X7R    | Input cap                           |
| C2        | 22 µF, 10V X7R     | Output smoothing cap                |
| C3        | 10 pF              | FB stability cap                    |
| K1–K4     | 2-pin headers      | Battery, solar input, jumper, output|

---

## 🖥️ Schematic & Working Principle

- **Daytime**: Sunlight charges the NiMH battery via D2 and disables the converter via T1.
- **Night**: T1 turns off, enabling IC1 to boost the battery to 3.3V.
- **Optional**: Skip T1 to have always-on output or control with jumper at K3.

![image](https://github.com/user-attachments/assets/c677532a-712e-420e-a906-0f6086edd822)
 <!-- Replace with your schematic -->

---

## 🚀 Usage Notes

1. Connect a small solar panel (3–6V open circuit) to `K4`.
2. Insert a 1.2V NiMH AA cell to `K2`.
3. Regulated 3.3V will be available at `K1` when solar input drops.
4. Use jumper or switch on `K3` to override automatic shutdown.

---


---

## 🔗 Reference

- 📰 Original article: [Elektor Labs – Tiny Solar Supply](https://elektormagazine.com/labs/tiny-solar-supply)
- 📄 AP3015 Datasheet: [Diodes Inc](https://www.diodes.com/assets/Datasheets/AP3015.pdf)

---

## 📄 License

This project is open-source under the [MIT License](../LICENSE).  
All design adaptations credited to the Elektor Lab article by Clemens Valens.

---

## 🙋‍♂️ Author & Contact

Designed and adapted by **Ruthvik Reddy A**  
📩 Email: `reddy.ruthvik0411@gmail.com`


