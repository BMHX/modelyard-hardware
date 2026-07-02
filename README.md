# 🔦 Forge 60

**Open-hardware 60 W / 10,000 lm DIY flashlight kit with USB-C power, active cooling, and full manufacturing files.**

[![License: CERN-OHL-P-2.0](https://img.shields.io/badge/License-CERN--OHL--P--2.0-blue.svg)](LICENSE)
[![Hardware: Open Source](https://img.shields.io/badge/Hardware-Open%20Source-brightgreen.svg)](#-hardware-downloads)
[![Demo: YouTube](https://img.shields.io/badge/Demo-YouTube-red.svg)](https://www.youtube.com/watch?v=xSCZzmICGlw)
[![Buy: ModelYard](https://img.shields.io/badge/Buy-ModelYard-black.svg)](https://modelyard.cc/products/forge-60)

Forge 60 is a reproducible open-hardware flashlight project built around a constant 60 W / 10,000 lm output mode, a high-current driver board, a 5050 LED board, active cooling, and a USB-C charge/discharge power path. Builders can manufacture the PCBs, source parts from the BOM, assemble the kit, flash the firmware, and modify the design.

## 🚀 Quick Links

| Action | Link |
| --- | --- |
| ▶️ Watch the demo | [YouTube: Forge 60 demo](https://www.youtube.com/watch?v=xSCZzmICGlw) |
| 🛒 Buy the kit | [modelyard.cc/products/forge-60](https://modelyard.cc/products/forge-60) |
| 📦 Download release package | [GitHub Releases](https://github.com/BMHX/modelyard-hardware/releases) |
| 🧩 Download hardware files | [Hardware Downloads](#-hardware-downloads) |
| 🛠️ Edit source project | [EasyEDA Pro source](forge60-hardware-release/source/forge60-easyeda-pro-source.epro2) |

![Forge 60 product photo](assets/images/forge60-product-1.jpg)

## 📚 Contents

- [Highlights](#-highlights)
- [Demo Video](#-demo-video)
- [Buy the Kit](#-buy-the-kit)
- [Performance](#-performance)
- [Specifications](#-specifications)
- [Hardware Downloads](#-hardware-downloads)
- [PCB and Schematic Preview](#-pcb-and-schematic-preview)
- [BOM Overview](#-bom-overview)
- [Required Tools](#-required-tools)
- [Firmware Flashing](#-firmware-flashing)
- [Assembly Notes](#-assembly-notes)
- [Safety Notes](#-safety-notes)
- [Repository Layout](#-repository-layout)
- [License](#-license)

## ✨ Highlights

- ⚡ Constant 60 W high-output flashlight platform
- 💡 About 10,000 lm output, depending on LED selection and thermal setup
- 🔌 45 W USB-C charging and discharging
- 🔋 2S 21700 battery pack architecture
- 🌬️ Active cooling with a 30 x 30 x 50 mm heatsink and 3010 fan
- 🧾 Complete Gerber, BOM, pick-and-place, schematic, and PCB preview files
- 🧰 EasyEDA Pro source project included for editing and modification
- 📜 CERN-OHL-P-2.0 permissive open hardware license

## ▶️ Demo Video

Click the preview below to watch the Forge 60 demo.

[![Forge 60 demo video](https://img.youtube.com/vi/xSCZzmICGlw/maxresdefault.jpg)](https://www.youtube.com/watch?v=xSCZzmICGlw)

Direct link: [https://www.youtube.com/watch?v=xSCZzmICGlw](https://www.youtube.com/watch?v=xSCZzmICGlw)

## 🛒 Buy the Kit

The project is fully open for builders who want to manufacture or modify it themselves. A ready-to-build kit is also available here:

### 👉 [Buy Forge 60 Kit on ModelYard](https://modelyard.cc/products/forge-60)

## ⏱️ Performance

| Mode | Runtime |
| --- | --- |
| 60 W | About 27 minutes |
| 30 W | About 54 minutes |
| 3 W | About 8 hours |

These figures are reference values from the project build. Final performance depends on LED bin, cells, protection board, wiring, cooling quality, firmware, and assembly.

## 📐 Specifications

| Item | Value |
| --- | --- |
| Project name | Forge 60 |
| Type | High-power DIY flashlight |
| Maximum power | 60 W |
| Optical output | About 10,000 lm |
| USB-C power | About 45 W charging / discharging |
| Battery architecture | 2S 21700 lithium battery pack |
| Recommended cells | High-drain 21700 cells, such as JP40 / 40PL / 45D class cells |
| Mainboard thickness | 1.0 mm |
| LED board thickness | 1.6 mm |
| Cooling | 30 x 30 x 50 mm heatsink + 3010 fan |
| Hardware license | CERN-OHL-P-2.0 |

## 📸 Photos

| Product | Product | Product |
| --- | --- | --- |
| ![Forge 60 product photo 1](assets/images/forge60-product-1.jpg) | ![Forge 60 product photo 2](assets/images/forge60-product-2.jpg) | ![Forge 60 product photo 3](assets/images/forge60-product-3.jpg) |

## 📦 Hardware Downloads

Gerber files are for PCB fabrication. BOM files are for sourcing. Pick-and-place files are for SMT assembly. The EasyEDA Pro source project is provided for editing and modification.

| Board | Gerber | BOM | Pick and Place | Schematic | PCB Preview |
| --- | --- | --- | --- | --- | --- |
| Mainboard v2 | [ZIP](forge60-hardware-release/mainboard-v2/mainboard-v2-gerber.zip) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.csv) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.csv) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-schematic.pdf) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-pcb-preview.pdf) |
| 5050 LED Board | [ZIP](forge60-hardware-release/led-board-5050/led-board-5050-gerber.zip) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-bom.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-bom.csv) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.csv) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-schematic.pdf) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-pcb-preview.pdf) |

## 🧩 Source Project

| Format | Download |
| --- | --- |
| EasyEDA Pro source | [forge60-easyeda-pro-source.epro2](forge60-hardware-release/source/forge60-easyeda-pro-source.epro2) |

## 🧭 PCB and Schematic Preview

### PCB Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 PCB preview](assets/pcb/mainboard-v2-pcb-preview.png) | ![5050 LED board PCB preview](assets/pcb/led-board-5050-pcb-preview.png) |

### Schematic Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 schematic](assets/schematics/mainboard-v2-schematic.png) | ![5050 LED board schematic](assets/schematics/led-board-5050-schematic.png) |

## 🧾 BOM Overview

The full BOM is provided in the hardware download table. Major parts include:

- IP2369 charge/discharge controller
- FP7209 LED driver controller
- PY32F003 series MCU
- 5050 6 V LEDs, 5000 K / 5700 K recommended
- 2S protection board, 13 A class recommended
- High-drain 21700 cells, such as JP40 / 40PL / 45D class cells
- 30 x 30 x 50 mm heatsink
- 3010 cooling fan
- 74 mm protective glass
- XT30 male/female connectors
- GH1.25 2P cables
- 20 AWG and 16 AWG flexible silicone wires
- M1.4 and M1.7 heat-set inserts
- Matching hex screws and self-tapping screws
- Reflective film, thermal tape, thermal grease, shock-absorbing foam, and high-temperature tape

## 🧰 Required Tools

- 3D printer
- Spot welder
- Hot plate or hot air station
- Soldering iron
- PWLINK2 LITE programmer
- 1.25 mm programming probe
- Glass cutter, if cutting the protective glass manually
- H1.3 / H1.5 hex drivers

## 💾 Firmware Flashing

Use PWLINK2 LITE and select the PY32F003xx6 series target in the programming software. Pay close attention to the V and G pads on the mainboard. Reversed programming probe wiring can damage the board.

| Select MCU | Add firmware | Apply firmware |
| --- | --- | --- |
| ![Select chip](assets/build/firmware-chip-select.png) | ![Add firmware](assets/build/firmware-add-file.png) | ![Apply firmware](assets/build/firmware-apply.png) |

| Probe wiring | Mainboard pads | Program complete |
| --- | --- | --- |
| ![Programming probe wiring](assets/build/programming-probe-wiring.jpg) | ![Programming probe pads](assets/build/programming-test-pads.png) | ![Firmware program success](assets/build/firmware-program-success.png) |

## 🔧 Assembly Notes

1. Flash the mainboard firmware before final assembly.
2. Use 16 AWG silicone wire for the mainboard input and XT30 male connector.
3. Use 20 AWG silicone wire and GH1.25 2P cables on the LED board side.
4. Mount the 3010 fan to the heatsink, then modify the fan lead to GH1.25 2P if needed.
5. Connect the mainboard output, LED board input, temperature sensing line, and fan line before closing the structure.
6. Use M1.7 heat-set inserts for the lamp-head top cover and M1.4 heat-set inserts for the handle connection.
7. Center the protection board inside the handle battery pack.
8. Add foam around the battery pack output side to reduce vibration and compression risk.

| Mainboard input wiring | Fan installation | Fan connector modification |
| --- | --- | --- |
| ![Mainboard input wires](assets/build/mainboard-input-wires.jpg) | ![Fan mounted on heatsink](assets/build/fan-mounted-on-heatsink.jpg) | ![Fan connector modification](assets/build/fan-connector-mod.jpg) |

| Mainboard and LED board wiring | Battery pack installation |
| --- | --- |
| ![Mainboard and LED board wiring](assets/build/mainboard-led-board-wiring.jpg) | ![Battery pack installation](assets/build/battery-pack-installation.jpg) |

## 🎛️ Operation

![Forge OS v1.2 instructions](assets/build/forge-os-v1.2-instructions.jpg)

## ⚠️ Safety Notes

This is a high-power LED and lithium battery project. Build and test it carefully.

- Do not downgrade protection board, cell, wire, or connector specifications.
- Verify the thermal path before sustained high-power operation.
- Check polarity and programming probe orientation before flashing.
- Current-limit the first power-on test and monitor temperature.
- Do not leave the battery pack or high-power LED unattended during early testing.
- If shipping batteries internationally, use a logistics channel that supports lithium batteries.

## 🗂️ Repository Layout

```text
forge60-hardware-release/
  mainboard-v2/
    mainboard-v2-gerber.zip
    mainboard-v2-bom.xlsx
    mainboard-v2-bom.csv
    mainboard-v2-pick-and-place.xlsx
    mainboard-v2-pick-and-place.csv
    mainboard-v2-schematic.pdf
    mainboard-v2-pcb-preview.pdf
  led-board-5050/
    led-board-5050-gerber.zip
    led-board-5050-bom.xlsx
    led-board-5050-bom.csv
    led-board-5050-pick-and-place.xlsx
    led-board-5050-pick-and-place.csv
    led-board-5050-schematic.pdf
    led-board-5050-pcb-preview.pdf
  source/
    forge60-easyeda-pro-source.epro2
```

## 📜 License

This hardware project is released under the CERN Open Hardware Licence Version 2 - Permissive (`CERN-OHL-P-2.0`). Commercial use is allowed under the terms of the license.
