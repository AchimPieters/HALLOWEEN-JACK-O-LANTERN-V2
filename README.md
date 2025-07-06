# HALLOWEEN-JACK-O-LANTERN-V2
 Halloween – Jack O’ Lantern V2: Ultimate Fire Effect

This project is a next-level version of the original [Jack O’ Lantern](#) flickering flame. It uses an ATtiny85 and six individually controlled LEDs to simulate a more realistic and dynamic fire effect — perfect for Halloween decorations, cosplay props, fantasy builds, and magical scenes.

Now with optional *blue flame mode* for a magical, Harry Potter–inspired effect!

---

##  Features

- Powered by ATtiny85 microcontroller  
- 6 individually PWM-controlled LEDs (3× red, 3× yellow)
- Realistic flame flicker with bursts and glow
- Smooth, natural-looking transitions using logarithmic fading
- Optional **Blue Flame Mode** (v2.1.0) using neon blue LED's
- Compact custom PCB included for easy assembly
- Low power – runs on 3×AA batteries

---

##  Bill of Materials

| Qty | Component               |
|-----|-------------------------|
| 1   | ATtiny85 microcontroller |
| 6   | 200Ω resistors           |
| 3   | 3mm Red LED's             |
| 3   | 3mm Yellow LED's          |
| 1   | 3×AA battery holder with switch |
| 3   | AA batteries             |
| 1   | Custom PCB (included in repo) |

Want a magical look? Swap all LED's for **neon blue** versions in firmware v2.1.0.

---

## PCB & Schematic

This repository includes:

- **KiCad project files**
- **Schematic (.sch)**
- **PCB layout (.kicad_pcb)**
- **Gerber files** for manufacturing
- **Render preview** of the assembled board

---

## Circuit Diagram

All LED's are connected to PWM-capable pins on the ATtiny85:  
`PB0–PB5` are used for controlling individual LED's.

> **Note:** `PB5` (pin 1) is the default RESET pin.  
> If you want to use it as output, you'll need to disable RESET via **RSTDISBL fuse**, which requires high voltage programming for future re-flashing.

---

## 3D model


### Regular Setup
<img src="https://raw.githubusercontent.com/AchimPieters/HALLOWEEN-JACK-O-LANTERN-V2/main/PCB_3D.png" style="height:200px;" />

### Neonblue Setup
<img src="https://raw.githubusercontent.com/AchimPieters/HALLOWEEN-JACK-O-LANTERN-V2/main/NEONBLUE.png" style="height:190px;" />



---

## Programming

You can flash the ATtiny85 using any of the following:

- USBasp
- TinyUSB programmer
- Arduino as ISP

Upload the included `.ino` file or compile from source. Programming tools like `avrdude`, `AVRDUDE GUI`, or the Arduino IDE (with core support) will work.

---

## Usage

| Firmware Version | Description                          |
|------------------|--------------------------------------|
| v2.0.0           | Warm flickering with red/yellow LED's|
| v2.1.0           | Cool magical flame with blue LED's   |

- Solder components onto the PCB
- Insert the programmed ATtiny85
- Connect the battery pack and flip the switch

Enjoy your realistic or magical LED fire effect!

---
