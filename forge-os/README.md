# Forge OS

Forge OS is the firmware that runs Forge 60, Forge 65, Forge 66, and Forge 201. It targets the PY32F003 series MCU on the mainboard and is distributed as Intel HEX files.

[← All ModelYard hardware projects](../README.md)

> Forge OS is distributed as compiled HEX files only. The firmware source code is not published.

## Which File to Flash

| Light | Version | File | Notes |
| --- | --- | --- | --- |
| Forge 60 | v1.2 | [forge60-os-v1.2.hex](../forge60/firmware/forge60-os-v1.2.hex) | |
| Forge 65 / Forge 66 | v1.2.2 | [forge-os-forge65-66-v1.2.2-standard.hex](../forge65/firmware/forge-os-forge65-66-v1.2.2-standard.hex) | Start here |
| Forge 65 / Forge 66 | v1.2.2 | [forge-os-forge65-66-v1.2.2-fine-tune-minus-2.hex](../forge65/firmware/forge-os-forge65-66-v1.2.2-fine-tune-minus-2.hex) | Power fine-tune −2 relative to standard |
| Forge 201 | v1.2.3 | [forge-os-forge201-v1.2.3-standard.hex](../forge201/firmware/forge-os-forge201-v1.2.3-standard.hex) | Start here |
| Forge 201 | v1.2.3 | [forge-os-forge201-v1.2.3-fine-tune-plus-2.hex](../forge201/firmware/forge-os-forge201-v1.2.3-fine-tune-plus-2.hex) | Power fine-tune +2 |
| Forge 201 | v1.2.3 | [forge-os-forge201-v1.2.3-fine-tune-plus-4.hex](../forge201/firmware/forge-os-forge201-v1.2.3-fine-tune-plus-4.hex) | Power fine-tune +4 |
| Forge 201 | v1.2.3 | [forge-os-forge201-v1.2.3-fine-tune-minus-2.hex](../forge201/firmware/forge-os-forge201-v1.2.3-fine-tune-minus-2.hex) | Power fine-tune −2 |

Flash the standard build first. The fine-tune builds shift the output power up (+) or down (−) relative to the standard build.

Forge 500 uses a different controller and firmware; see [Forge 500](../forge500/README.md).

## Flashing

Use a PWLINK2 LITE programmer, select the PY32F003xx6 target, load the HEX file, and program. Check the V and G pads before connecting the probe: reversed probe wiring can damage the board.

The step-by-step screenshots and probe photos are in the [Forge 60 firmware flashing guide](../forge60/README.md#firmware-flashing).

## Operation (v1.2)

| Action | Result |
| --- | --- |
| Long press | Power on / off. After power-on, the three indicator LEDs show the battery level. |
| Keep holding after power-on | Strobe; release to exit |
| Single click while on | Switch output level |
| Double click while off | Double flash; brightness follows the current level |
| Triple click while off | Toggle between 3-level and 5-level mode |
| Five clicks while off | Lock / unlock |

Indicator patterns:

- 3-level mode selected: the indicator LEDs flash in the 3-level pattern.
- 5-level mode selected: the indicator LEDs flash in the 5-level pattern.
- Locked / unlocked: each has its own flash pattern.

The photos of each pattern are in the original user guide image: [forge-os-v1.2-user-guide-zh.jpg](forge-os-v1.2-user-guide-zh.jpg) (Chinese).

**Maximum level limit:** while the charging indicator is lit, the highest output level is unavailable. It becomes available again once the charging indicator turns off.
