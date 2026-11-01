# LORENTZ
An all-analog topology complex oscillator inspired by Don Buchla’s 259. Sized for Eurorack (28 HP).  

![LORENTZ REV-A front panels, off-white and black][image-1]

## Overview
Two oscillators, a modulation oscillator and a principal oscillator:
- **Modulation oscillator:** coarse tuning dial (-3 to +3), SYMM, WAVE and FREQ, AM, MOD OUTS (two waveforms).
- **Principal oscillator:** coarse tuning dial (-3 to +3), FINE, PITCH and EXP CV inputs, TIMBRE, PRINC OUTS (two waveforms).
- **Modulation:** INDEX, with an EXP/LIN toggle.
- **Waveshaping:** SHAPE, with a FINAL output.
## Front panel
- Eurorack 3U x 28 HP: **141.9 x 128.5 mm**, square corners.
- **2.0 mm** 5052 (or 6061) aluminium.
- **39 holes + 4 rail slots.**

| Feature         | Qty | Dia (mm)                                 | Part                                   |
| --------------- | --- | ---------------------------------------- | -------------------------------------- |
| Pot bushings    | 8   | 7.3                                      | Alpha 9 mm x6, Alpha RV16 x2 (M7x0.75) |
| Jacks           | 13  | 6.3                                      | Thonkiconn PJ398SM (M6)                |
| Toggle          | 1   | 5.2                                      | Dailywell 2MD1T1B1M2QES (10-48 UNS)    |
| LEDs            | 11  | 3.2                                      | 3 mm LED, lens flush                   |
| Standoff screws | 6   | 3.4 thru + 90° countersink Ø6.0 on front | M3x6 DIN 965 / ISO 7046 countersunk    |
| Rail slots      | 4   | 5.6 x 3.2 stadium                        | M3 rail screws                         |

Colourways:

| Version   | Base           | Ink                 | Accents                    |
| --------- | -------------- | ------------------- | -------------------------- |
| Off-white | \#E9E6DC matte | \#2A1404 dark brown | red #D8302A, amber #ECB731 |
| Black     | \#2C2C2C matte | white               | red #D8302A, amber #ECB731 |

Full details, including countersink depth and print registration, are in `panel/<colour>/PANEL_FAB_SPEC.md`.
## Fabrication
**PCBs.** Zip and upload each gerber folder separately:
- `control_board/gerbers/` (12 files: 4 copper, mask, silk, edge, drill + map, job)
- `circuit_board/gerbers/` (same)
**Panel.**
1. Cut and drill from `panel/<colour>/panel_REV-A_cut.dxf` (mm, origin bottom-left; layers `CUT` and `CSK_FRONT_6.0x90`). `panel_REV-A_cut.svg` is the same geometry.
2. Countersink the six standoff holes first, then UV-print.
3. Print from `panel/<colour>/LORENTZ_REV-A_print_<colour>_outlined.svg`. Register to the hole centers in `panel_REV-A_holes.csv` within ±0.2 mm.
Ask the fab for a color proof against the base color.
## Bill of materials
See `bom/`. `LORENTZ_REV-A_build1_BOM.csv` lists suppliers and part numbers for a single build. `LORENTZ_REV-A_BOM_x5.csv` covers five builds. The `*_bom_from_sch.csv` files are fresh exports from the schematics.
## License
Apache 2.0

[image-1]:	images/LORENTZ_REV-A_offwhite.png
