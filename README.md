# Forge 60

Forge 60 is a compact high-power DIY flashlight designed for a constant 60 W / 10,000 lm output mode. It supports 45 W USB-C charging and discharging, charges in about one hour, and is designed as an open hardware kit that builders can assemble, inspect, modify, and manufacture.

![Forge 60 product photo](assets/images/forge60-product-1.jpg)

## Key Specs

| Item | Value |
| --- | --- |
| Output mode | 60 W / 10,000 lm |
| USB-C power | 45 W charging / discharging |
| Full charge time | About 1 hour |
| Runtime at 60 W | About 27 minutes |
| Runtime at 30 W | About 54 minutes |
| Runtime at 3 W | About 8 hours |
| Mainboard thickness | 1.0 mm |
| LED board thickness | 1.6 mm |
| Hardware license | CERN-OHL-P-2.0 |

## Photos

| Product | Product | Product |
| --- | --- | --- |
| ![Forge 60 front](assets/images/forge60-product-1.jpg) | ![Forge 60 side](assets/images/forge60-product-2.jpg) | ![Forge 60 rear](assets/images/forge60-product-3.jpg) |

## Hardware Downloads

Use the table below to download the files directly. Gerber files are for PCB fabrication. BOM and pick-and-place files are for sourcing and SMT assembly. The EasyEDA Pro source project is provided for editing.

| Board | Gerber | BOM | Pick and Place | Schematic | PCB Preview |
| --- | --- | --- | --- | --- | --- |
| Mainboard v2 | [ZIP](forge60-hardware-release/mainboard-v2/mainboard-v2-gerber.zip) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-bom.csv) | [XLSX](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.xlsx) / [CSV](forge60-hardware-release/mainboard-v2/mainboard-v2-pick-and-place.csv) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-schematic.pdf) | [PDF](forge60-hardware-release/mainboard-v2/mainboard-v2-pcb-preview.pdf) |
| 5050 LED Board | [ZIP](forge60-hardware-release/led-board-5050/led-board-5050-gerber.zip) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-bom.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-bom.csv) | [XLSX](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.xlsx) / [CSV](forge60-hardware-release/led-board-5050/led-board-5050-pick-and-place.csv) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-schematic.pdf) | [PDF](forge60-hardware-release/led-board-5050/led-board-5050-pcb-preview.pdf) |

## Source Project

| Format | Download |
| --- | --- |
| EasyEDA Pro source | [forge60-easyeda-pro-source.epro2](forge60-hardware-release/source/forge60-easyeda-pro-source.epro2) |

## PCB Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 PCB preview](assets/pcb/mainboard-v2-pcb-preview.png) | ![5050 LED board PCB preview](assets/pcb/led-board-5050-pcb-preview.png) |

## Schematic Preview

| Mainboard v2 | 5050 LED Board |
| --- | --- |
| ![Mainboard v2 schematic](assets/schematics/mainboard-v2-schematic.png) | ![5050 LED board schematic](assets/schematics/led-board-5050-schematic.png) |

## Repository Layout

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

## License

This hardware project is released under the CERN Open Hardware Licence Version 2 - Permissive (`CERN-OHL-P-2.0`). Commercial use is allowed under the terms of the license.
