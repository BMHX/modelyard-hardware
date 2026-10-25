# Forge 201

Actively cooled 200 W / about 30,000 lm flashlight that holds full output without a planned step-down, powered by a 4S 21700 pack.

[← All ModelYard hardware projects](../README.md)

<p align="center">
  <img src="../assets/products/forge201.png" width="320" alt="Forge 201 reflector and LED">
</p>

## At a Glance

| Item | Value |
| --- | --- |
| Output | 200 W / about 30,000 lm |
| Runtime | About 19 min at 200 W, 5 h at 15 W |
| LED | CXM32, 6500 K, Ra70 |
| Power control | IP2369 with a CMSA070N10 main MOSFET |
| Battery | 4S 21700 pack with an NTC protection board (50 A recommended, 25 A minimum), XT30 lead |
| Cooling | 50 x 50 x 50 mm heatsink + 5010 fan |
| Front glass | 74 mm coated glass |
| Weight | About 720 g |

## What Is in This Folder

| File | Use |
| --- | --- |
| [mechanical/forge201-v1.0.3mf](mechanical/forge201-v1.0.3mf) | Bambu Studio project: lamp head, handle, top cap, tail cap, button |
| [mechanical/forge201-stl-v1.0.zip](mechanical/forge201-stl-v1.0.zip) | STL files for the same parts |
| [mechanical/forge201-f3d-v1.0.zip](mechanical/forge201-f3d-v1.0.zip) | Fusion 360 source for the same parts |
| [mechanical/forge201-reflective-film-mold.stl](mechanical/forge201-reflective-film-mold.stl) | Mold for forming the reflective film |
| [firmware/forge-os-forge201-v1.2.3-standard.hex](firmware/forge-os-forge201-v1.2.3-standard.hex) | Forge OS v1.2.3, start here |
| [firmware/forge-os-forge201-v1.2.3-fine-tune-plus-2.hex](firmware/forge-os-forge201-v1.2.3-fine-tune-plus-2.hex) | Power fine-tune +2 |
| [firmware/forge-os-forge201-v1.2.3-fine-tune-plus-4.hex](firmware/forge-os-forge201-v1.2.3-fine-tune-plus-4.hex) | Power fine-tune +4 |
| [firmware/forge-os-forge201-v1.2.3-fine-tune-minus-2.hex](firmware/forge-os-forge201-v1.2.3-fine-tune-minus-2.hex) | Power fine-tune −2 |

Flashing and button operation: see [Forge OS](../forge-os/README.md).

**Not included yet:** PCB files for Forge 201.

## Buy Assembled

[modelyard.cc/products/forge-201](https://modelyard.cc/products/forge-201)

## Safety

At 200 W this light draws high current from a 4S pack. Use a built pack with an NTC-equipped protection board, current-limit the first power-on, and monitor temperature.

## License

CC BY-NC-SA 4.0. Commercial use requires written permission; see [License](../README.md#license).
