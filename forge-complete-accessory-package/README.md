# Forge Complete Accessory Package

This folder contains additional Forge-series accessory resources, 3D files, firmware files, stencil files, and source model files.

These files are provided as an auxiliary resource package. For the primary Forge 60 PCB manufacturing files, BOM, schematic, firmware, and main mechanical model, use the main release folder:

[../forge60-hardware-release](../forge60-hardware-release)

## Package Contents

| Folder | Contents |
| --- | --- |
| `Forge60Mecha_Edition/` | Forge 60 Mecha Edition Fusion 360 source, STL package, 3MF package, extended handle STL, and add-on 3MF |
| `Forge65 3D_Files/` | Forge 65 3MF files, STL package, extended handle 3MF, and 8-cell package |
| `Forge60 65Stencil/` | Forge 60 v2 mainboard stencil DXF |
| `Forge200 3D_Models/` | Forge 200 Fusion 360 source files, STL files, and 3MF files |
| `Forgeos Firmware/` | Forge OS firmware HEX files for Forge 60, Forge 65/66, and Forge 201, plus user guide images |
| `Forge500/` | Forge 500 UF2 firmware files, print files, Fusion 360 source, add-ons, and offline replication document |
| `Forge201 3D_Files/` | Forge 201 STL package, Fusion 360 source package, 3MF file, and reflective film mold STL |

## Notes

- File names are kept close to the original exported names to preserve compatibility with external references.
- Some files are model-source or slicer/project files, such as `.f3d`, `.f3z`, `.3mf`, `.stl`, `.dxf`, `.hex`, `.uf2`, `.zip`, `.jpg`, and `.mhtml`.
- Verify firmware target model and hardware revision before flashing.
- Verify print orientation, material, inserts, and thermal requirements before printing or assembling.
