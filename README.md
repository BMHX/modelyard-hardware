<h1 align="center">Forge 60</h1>

<p align="center">
  <strong>Open-hardware 60 W / 10,000 lm DIY flashlight kit with USB-C power, active cooling, and full manufacturing files.</strong>
</p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=xSCZzmICGlw"><img alt="Watch on YouTube" src="https://img.shields.io/badge/Watch-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white"></a>
  <a href="https://modelyard.cc/products/forge-60"><img alt="Buy on ModelYard" src="https://img.shields.io/badge/Buy%20Kit-ModelYard-111111?style=for-the-badge"></a>
  <a href="https://discord.com/invite/2pjCQccBc"><img alt="Join Discord" src="https://img.shields.io/badge/Join-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white"></a>
  <a href="https://github.com/BMHX/modelyard-hardware/releases"><img alt="Download release" src="https://img.shields.io/badge/Download-Release-2ea44f?style=for-the-badge&logo=github&logoColor=white"></a>
</p>

<p align="center">
  <a href="LICENSE"><img alt="License: CERN-OHL-P-2.0" src="https://img.shields.io/badge/License-CERN--OHL--P--2.0-blue.svg"></a>
  <a href="#hardware-downloads"><img alt="Open hardware files" src="https://img.shields.io/badge/Hardware%20Files-Gerber%20%7C%20BOM%20%7C%20CPL%20%7C%20Schematic-lightgrey.svg"></a>
  <a href="#source-project"><img alt="EasyEDA Pro source" src="https://img.shields.io/badge/Source-EasyEDA%20Pro-orange.svg"></a>
</p>

![Forge 60 product photo](assets/images/forge60-product-1.jpg)

Forge 60 is a reproducible open-hardware flashlight platform built around a constant 60 W / 10,000 lm output mode, a high-current driver board, a 5050 LED board, active cooling, and a USB-C charge/discharge power path. The repository includes fabrication files, assembly data, schematics, and editable EasyEDA Pro source files so builders can manufacture, inspect, modify, and assemble the project.

## At a Glance

| Item | Value |
| --- | --- |
| Output | 60 W / about 10,000 lm |
| USB-C power | About 45 W charging / discharging |
| Battery architecture | 2S 21700 lithium battery pack |
| Cooling | 30 x 30 x 50 mm heatsink + 3010 fan |
| Recommended hardware files | Mainboard v2 + 5050 LED board |
| Mainboard thickness | 1.0 mm |
| LED board thickness | 1.6 mm |
| Firmware | Forge 60 OS v1.2 HEX |
| Mechanical model | Forge 60 v10 3MF |
| Source format | EasyEDA Pro `.epro2` |
| License | CERN-OHL-P-2.0 |

## Important Notes

- **Recommended board:** use `mainboard-v2`. Older mainboard revisions are not recommended for new builds.
- **PCB thickness matters:** order the mainboard at **1.0 mm** and the LED board at **1.6 mm**.
- **KiCad is not included yet:** editable source is currently provided as an EasyEDA Pro project.
- **High-power safety:** this project uses high-current lithium cells and a high-power LED. Validate wiring, polarity, thermal path, and firmware before sustained operation.
- **Battery shipping:** if you ship kits with cells, use a logistics channel that supports lithium batteries.

## Quick Links

| Action | Link |
| --- | --- |
| <img src="assets/icons/youtube.svg" width="18" alt="YouTube"> Watch demo | [YouTube video](https://www.youtube.com/watch?v=xSCZzmICGlw) |
| <img src="assets/icons/modelyard.svg" width="18" alt="ModelYard"> Buy kit | [ModelYard Forge 60 kit](https://modelyard.cc/products/forge-60) |
| <img src="assets/icons/discord.svg" width="18" alt="Discord"> Join community | [Discord invite](https://discord.com/invite/2pjCQccBc) |
| <img src="assets/icons/github.svg" width="18" alt="GitHub"> Download release | [GitHub Releases](https://github.com/BMHX/modelyard-hardware/releases) |
| Download hardware files | [Hardware Downloads](#hardware-downloads) |
| Download firmware | [Forge 60 OS v1.2 HEX](forge60-hardware-release/firmware/forge60-os-v1.2.hex) |
| Download mechanical model | [Forge 60 v10 3MF](forge60-hardware-release/mechanical/forge60-v10.3mf) |
| Edit source project | [EasyEDA Pro source](forge60-hardware-release/source/forge60-easyeda-pro-source.epro2) |

## Contents

- [Demo](#demo)
- [Kit Availability](#kit-availability)
- [Performance](#performance)
- [Hardware Downloads](#hardware-downloads)
- [Manufacturing Notes](#manufacturing-notes)
- [Firmware and Mechanical Files](#firmware-and-mechanical-files)
- [Source Project](#source-project)
- [PCB and Schematic Preview](#pcb-and-schematic-preview)
- [BOM Overview](#bom-overview)
- [Build Flow](#build-flow)
- [Firmware Flashing](#firmware-flashing)
- [Assembly Notes](#assembly-notes)
- [Safety and Disclaimer](#safety-and-disclaimer)
- [Repository Layout](#repository-layout)
- [License](#license)

## Demo

[![Forge 60 demo video](https://img.youtube.com/vi/xSCZzmICGlw/hqdefault.jpg)](https://www.youtube.com/watch?v=xSCZzmICGlw)

Watch the demo: [https://www.youtube.com/watch?v=xSCZzmICGlw](https://www.youtube.com/watch?v=xSCZzmICGlw)

## Kit Availability

This repository contains the open hardware files for builders who want to manufacture or modify the project themselves. A ready-to-build kit is available separately:

[![Buy Forge 60 Kit on ModelYard](https://img.shields.io/badge/Buy%20Forge%2060%20Kit-ModelYard-111111?style=for-the-badge)](https://modelyard.cc/products/forge-60)

Direct link: [https://modelyard.cc/products/forge-60](https://modelyard.cc/products/forge-60)

## Performance

| Mode | Runtime |
| --- | --- |
| 60 W | About 27 minutes |
| 30 W | About 54 minutes |
| 3 W | About 8 hours |

These are reference values from the project build. Final performance depends on LED bin, cell condition, protection board, wiring resistance, cooling quality, firmware, and assembly.

## Hardware Downloads

Gerber files are for PCB fabrication. BOM files are for sourcing. Pick-and-place files are for SMT assembly. Schematic and PCB preview files are provided for review.

| Board | Gerber | BOM | Pick and Place | Schematic | PCB Preview |
| --- | --- | --- | --- | --- | --- |
| Mainboard v2 | [ZIP](forge60-hardware-release/mainboard-v2/mainboard-v2-gerber.zip) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.csv) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.csv) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-schematic.pdf) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-pcb-preview.pdf) |
| 5050 LED Board | [ZIP](forge60-hardware-release/led-board-5050/led-board-5050-gerber.zip) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-bom.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-bom.csv) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.csv) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-schematic.pdf) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-pcb-preview.pdf) |

## Manufacturing Notes

- Mainboard v2: order as **1.0 mm** PCB.
- 5050 LED board: order as **1.6 mm** PCB.
- Use the Gerber zip, BOM, and pick-and-place files from the same board folder.
- The BOM files are the source of truth for electronic components; verify substitutes before assembly.
- If outsourcing SMT, provide the manufacturer with Gerber, BOM, and pick-and-place files together.

## Firmware and Mechanical Files

| File | Link | Use |
| --- | --- | --- |
| Forge 60 OS v1.2 firmware | [forge60-os-v1.2.hex](forge60-hardware-release/firmware/forge60-os-v1.2.hex) | Flash the PY32F003xx6 mainboard MCU |
| Forge 60 v10 mechanical model | [forge60-v10.3mf](forge60-hardware-release/mechanical/forge60-v10.3mf) | 3D-printable mechanical shell/model package |

## Source Project

| Format | Download |
| --- | --- |
| EasyEDA Pro source | [forge60-easyeda-pro-source.epro2](forge60-hardware-release/source/forge60-easyeda-pro-source.epro2) |

The editable project is currently provided in EasyEDA Pro format. KiCad files are not included in this release.

## PCB and Schematic Preview

### PCB Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 PCB preview](assets/pcb/mainboard-v2-pcb-preview.png) | ![5050 LED board PCB preview](assets/pcb/led-board-5050-pcb-preview.png) |

### Schematic Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 schematic](assets/schematics/mainboard-v2-schematic.png) | ![5050 LED board schematic](assets/schematics/led-board-5050-schematic.png) |

## BOM Overview

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
- Reflective film, thermal tape, thermal grease, shock-absorbing foam, and high-temperature tape

## Build Flow

1. Review the schematic PDFs and PCB previews.
2. Order the mainboard and LED board using the Gerber files and thickness notes.
3. Source components from the BOM.
4. Use pick-and-place files for SMT assembly where applicable.
5. Print or prepare the mechanical parts and cooling stack.
6. Flash the mainboard firmware.
7. Assemble wiring, LED board, fan, battery pack, and enclosure.
8. Perform current-limited first power-on testing and monitor temperature.

## Required Tools

- 3D printer
- Spot welder
- Hot plate or hot air station
- Soldering iron
- PWLINK2 LITE programmer
- 1.25 mm programming probe
- Glass cutter, if cutting the protective glass manually
- H1.3 / H1.5 hex drivers

## Firmware Flashing

Use PWLINK2 LITE and select the PY32F003xx6 series target in the programming software. Pay close attention to the V and G pads on the mainboard. Reversed programming probe wiring can damage the board.

| Select MCU | Add firmware | Apply firmware |
| --- | --- | --- |
| ![Select chip](assets/build/firmware-chip-select.png) | ![Add firmware](assets/build/firmware-add-file.png) | ![Apply firmware](assets/build/firmware-apply.png) |

| Probe wiring | Mainboard pads | Program complete |
| --- | --- | --- |
| ![Programming probe wiring](assets/build/programming-probe-wiring.jpg) | ![Programming probe pads](assets/build/programming-test-pads.png) | ![Firmware program success](assets/build/firmware-program-success.png) |

## Assembly Notes

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

## Operation

![Forge OS v1.2 instructions](assets/build/forge-os-v1.2-instructions.jpg)

## Community

For build discussion, support, updates, and modification ideas:

[![Join the Forge 60 Discord](https://img.shields.io/badge/Join%20Discord-Forge%2060%20Community-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/invite/2pjCQccBc)

Direct link: [https://discord.com/invite/2pjCQccBc](https://discord.com/invite/2pjCQccBc)

## Safety and Disclaimer

This is a high-power LED and lithium battery project. Build and test it carefully.

- Do not downgrade protection board, cell, wire, or connector specifications.
- Verify the thermal path before sustained high-power operation.
- Check polarity and programming probe orientation before flashing.
- Current-limit the first power-on test and monitor temperature.
- Do not leave the battery pack or high-power LED unattended during early testing.
- If shipping batteries internationally, use a logistics channel that supports lithium batteries.
- You are responsible for validating the design, assembly, firmware, battery pack, and thermal behavior before use.

## Repository Layout

```text
forge60-hardware-release/
  firmware/
    forge60-os-v1.2.hex
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
  mechanical/
    forge60-v10.3mf
  source/
    forge60-easyeda-pro-source.epro2
```

## License

This hardware project is released under the CERN Open Hardware Licence Version 2 - Permissive (`CERN-OHL-P-2.0`). Commercial use is allowed under the terms of the license.
