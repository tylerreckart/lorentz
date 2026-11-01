# LORENTZ (RECKART ELECTRON DYNAMICS TYPE R-28) front panel REV-A: fab spec

- **Material:** 5052 (or 6061) aluminium sheet, **2.0 mm** thick. Flat, deburred, no visible tool marks on the front.
- **Outline:** 141.9 × 128.5 mm (Eurorack 3U × 28 HP), square corners. Origin is top-left, front view, y down.
- **Finish:** off-white base **#E9E6DC**, matte.
  - **Preferred:** powder-coat or enamel the off-white, then **UV-print** the artwork (dark brown ink #2A1404, black hardware placeholders, red #D8302A LEDs/accents/footer mark, amber #ECB731 EXP/LIN LED rings) from `LORENTZ_REV-A_print_offwhite_outlined.svg`.
  - **Alternative:** full UV print (white base plus colour) on bare or anodised Al.
  - Ask the fab for a colour proof against #E9E6DC.
- **Artwork:** `LORENTZ_REV-A_print_offwhite_outlined.svg` (Tyler's final REV-A artwork, all text outlined; viewBox 536.315 × 485.669 px = 141.9 × 128.5 mm, so set the width to 141.9 mm). Do not scale. The black filled discs at hole positions are hardware placeholders and fall inside the cut-outs.
- **Cut/drill files:** `panel_REV-A_cut.dxf` (mm, origin bottom-left, layer CUT plus layer CSK_FRONT_6.0x90) and `panel_REV-A_cut.svg` (mm). Hole list: `panel_REV-A_holes.csv`.
- **Hole tolerance:** ±0.05 mm position, +0.1/−0 mm diameter.

| Feature | Qty | Dia (mm) | Part |
|---|---|---|---|
| Pot bushings | 8 | 7.3 | Alpha 9 mm ×6, Alpha RV16 ×2 (M7×0.75) |
| Jacks | 13 | 6.3 | Thonkiconn PJ398SM (M6) |
| Toggle | 1 | 5.2 | Dailywell 2MD1T1B1M2QES (10-48 UNS, 5.59 mm bushing) |
| LEDs | 11 | 3.2 | 3 mm LED, lens flush |
| Standoff screws | 6 | 3.4 thru + **90° countersink Ø6.0 on FRONT** | M3×6 DIN 965 / ISO 7046 countersunk, black |
| Rail slots | 4 | 5.6 × 3.2 stadium | M3 rail screws |

## Countersink for 2.0 mm stock
- **Screw:** DIN 965 / ISO 7046 M3 countersunk, black. Head Ø5.5 max, k = 1.65 mm.
- **Countersink:** 90° × Ø6.0 on the front face, 1.30 mm deep (from Ø3.4), leaving a **0.70 mm land**. Head sits ~0.2 mm below flush.
- **Do not use ISO 10642 hex socket heads** (Ø6.72, k = 1.86): ~0.1 mm land, pull-through risk.
- **Screw length:** M3×6 gives 4.0 mm engagement in the 10 mm F-F standoff.
- **Order: countersink first, then UV print.** The artwork's black Ø6.6 screw discs and printed rings cover the countersinks; ink on the cone is acceptable.
- Register the print to the hole centres in `panel_REV-A_holes.csv` within ±0.2 mm.

## Toggle fit caveat 
- The bushing shoulder sits ≈9.15 mm above the control PCB and the panel front is at 12.0 mm, so only ≈2.7 mm of thread protrudes. Use **one outer nut only** (plus the lock washer if it fits) and **no inner height-setting nut**. Check thread engagement on the first fit-up before tightening.

## REV-A panel notes
- New "final final" artwork from Tyler (offwhite version). Ink #2A1404 dark brown.
- As received, WAVE graphics were at x 28.70 (+0.30 mm), FREQ graphics at x 43.75 (+0.35 mm), toggle disc Ø6.5. Fixed: WAVE group (box, hatch, pale ring, disc, label) moved −0.30 mm in x; FREQ group (ring, disc, label, dotted arrow, arrowhead) −0.35 mm; toggle disc set to Ø5.2. Nothing else touched.
- After the fix all 39 holes are at 0.000 mm vs the board-derived hole list; no holes added or removed; no move over 1 mm.
- Footer: red logo mark 3.20 × 3.20 mm at (13.11, 123.88) mm; footer ink spans x 13.11–128.86 mm, clearing the rail slots by 2.81 mm (left) and 2.84 mm (right). The full-width footer rule (y 122.50 mm) clears the slot tops by 1.38 mm but runs edge to edge through the 3.5 mm side keep-out (Tyler's art, kept as drawn).
- Hole geometry unchanged (39 holes + 4 slots). No board changes driven by the art.
