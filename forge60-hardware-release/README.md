# Forge 60 Release

<p>
  <a href="https://github.com/BMHX/modelyard-hardware/releases/tag/v1.0.0"><img alt="GitHub Release" src="https://img.shields.io/badge/GitHub-Release-181717?logo=github&logoColor=white"></a>
  <a href="https://github.com/BMHX/modelyard-hardware/releases/download/v1.0.0/forge60-hardware-release-v1.0.0.zip"><img alt="Download release ZIP" src="https://img.shields.io/badge/Download-ZIP-0969DA?logo=github&logoColor=white"></a>
  <img alt="Release v1.0.0" src="https://img.shields.io/badge/Release-v1.0.0-blue">
  <img alt="License CERN-OHL-P-2.0" src="https://img.shields.io/badge/License-CERN--OHL--P--2.0-green">
</p>

Forge 60 is a compact high-power DIY flashlight project built around a 60 W class driver, a 5050 LED board, USB-C charging/discharging, active cooling, and a 2S 21700 battery pack.

This release packages the files needed to reproduce the electronics, flash the controller firmware, and print the mechanical shell.

## Release Metadata

| Item | Value |
| --- | --- |
| Release package | `forge60-hardware-release-v1.0.0.zip` |
| Hardware release | v1.0.0 |
| Mainboard | `mainboard-v2` |
| Firmware | Forge 60 OS v1.2 |
| Mechanical model | Forge 60 v10 |
| Source format | EasyEDA Pro |

## Download Release

| Package | Link | Use |
| --- | --- | --- |
| Full release ZIP | [GitHub Releases](https://github.com/BMHX/modelyard-hardware/releases/download/v1.0.0/forge60-hardware-release-v1.0.0.zip) | Download the complete hardware, firmware, and mechanical package |
| Release page | [Forge 60 v1.0.0](https://github.com/BMHX/modelyard-hardware/releases/tag/v1.0.0) | View release notes and attached assets |

## What Is Included

| Area | Folder | Contents |
| --- | --- | --- |
| Main control board | `mainboard-v2/` | Gerber, BOM, pick-and-place, schematic, PCB preview |
| 5050 LED board | `led-board-5050/` | Gerber, BOM, pick-and-place, schematic, PCB preview |
| Firmware | `firmware/` | Forge 60 OS firmware HEX |
| Mechanical model | `mechanical/` | 3D-printable 3MF model |
| Source project | `source/` | EasyEDA Pro source project |

## Recommended Order

1. Read the [safety notes](#safety).
2. Review the schematic and PCB preview PDFs in [Board Files](#board-files).
3. Order PCBs using the matching Gerber files.
4. Source parts from the matching BOM files.
5. Use the pick-and-place files for SMT assembly.
6. Print the [3MF mechanical model](#mechanical-model) and verify fitment.
7. Flash the [firmware](#firmware) before final assembly.

## Board Files

### Mainboard v2

| File | Link |
| --- | --- |
| Gerber | [mainboard-v2-gerber.zip](mainboard-v2/mainboard-v2-gerber.zip) |
| BOM | [XLSX](mainboard-v2/mainboard-v2-bom.xlsx) / [CSV](mainboard-v2/mainboard-v2-bom.csv) |
| Pick and place | [XLSX](mainboard-v2/mainboard-v2-pick-and-place.xlsx) / [CSV](mainboard-v2/mainboard-v2-pick-and-place.csv) |
| Schematic | [mainboard-v2-schematic.pdf](mainboard-v2/mainboard-v2-schematic.pdf) |
| PCB preview | [mainboard-v2-pcb-preview.pdf](mainboard-v2/mainboard-v2-pcb-preview.pdf) |

### 5050 LED Board

| File | Link |
| --- | --- |
| Gerber | [led-board-5050-gerber.zip](led-board-5050/led-board-5050-gerber.zip) |
| BOM | [XLSX](led-board-5050/led-board-5050-bom.xlsx) / [CSV](led-board-5050/led-board-5050-bom.csv) |
| Pick and place | [XLSX](led-board-5050/led-board-5050-pick-and-place.xlsx) / [CSV](led-board-5050/led-board-5050-pick-and-place.csv) |
| Schematic | [led-board-5050-schematic.pdf](led-board-5050/led-board-5050-schematic.pdf) |
| PCB preview | [led-board-5050-pcb-preview.pdf](led-board-5050/led-board-5050-pcb-preview.pdf) |

## Manufacturing Notes

| Item | Recommended setting |
| --- | --- |
| Mainboard version | `mainboard-v2` |
| Mainboard thickness | 1.0 mm |
| Mainboard layer count | 4 layers |
| LED board thickness | 1.6 mm |
| LED board package | 5050 LED layout |
| LED part | Seoul Semiconductor `STW0L8PA`, 6 V 5050, 5700 K, around CRI 70 |
| Assembly files | Use the matching BOM and pick-and-place files from the same board folder |

Before ordering, review the PCB preview PDF and confirm board stack-up, substrate, copper weight, surface finish, and assembly constraints with the PCB manufacturer.

The LED board BOM intentionally leaves the LED supplier part number blank because the current kit LED is not an LCSC part. Do not substitute the LED row with an 0805 indicator LED.

## Firmware

- Firmware file: [firmware/forge60-os-v1.2.hex](firmware/forge60-os-v1.2.hex)
- Target MCU family: PY32F003xx6
- Recommended programmer: PWLINK2 LITE

Check the programming probe orientation before flashing. Reversed V/G wiring can damage the mainboard.

## Mechanical Model

- 3MF model: [mechanical/forge60-v10.3mf](mechanical/forge60-v10.3mf)

Verify fitment against your printed material, printer tolerance, heat-set insert size, fan, heatsink, wiring length, and battery pack before final assembly.

## Source Project

- EasyEDA Pro source: [source/forge60-easyeda-pro-source.epro2](source/forge60-easyeda-pro-source.epro2)

Use the source project when you need to inspect or modify the schematic, PCB layout, BOM, or fabrication outputs.

## Repository Layout

```text
forge60-hardware-release/
  firmware/
    forge60-os-v1.2.hex
  led-board-5050/
    led-board-5050-bom.csv
    led-board-5050-bom.xlsx
    led-board-5050-gerber.zip
    led-board-5050-pcb-preview.pdf
    led-board-5050-pick-and-place.csv
    led-board-5050-pick-and-place.xlsx
    led-board-5050-schematic.pdf
  mainboard-v2/
    mainboard-v2-bom.csv
    mainboard-v2-bom.xlsx
    mainboard-v2-gerber.zip
    mainboard-v2-pcb-preview.pdf
    mainboard-v2-pick-and-place.csv
    mainboard-v2-pick-and-place.xlsx
    mainboard-v2-schematic.pdf
  mechanical/
    forge60-v10.3mf
  source/
    forge60-easyeda-pro-source.epro2
```

## Safety

This is a high-power LED and lithium battery project. Use current-limited first power-on testing, verify polarity, monitor temperature, and do not downgrade the battery, protection board, wire, connector, or cooling specifications.

## License

This hardware project is released under the CERN Open Hardware Licence Version 2 - Permissive (`CERN-OHL-P-2.0`). Commercial use is allowed under the terms of the license.
