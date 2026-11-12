RCA OUTPUT UPDATE
=================

The previous dual CAX connector has been replaced with two widely available
Same Sky / CUI RCJ-01X family single RCA jacks.

J3: RCJ-012 (red), JLC/LCSC C4991691
J4: RCJ-013 (white), JLC/LCSC C4992378
Footprint: Odderon:RCA_CUI_RCJ-01X_RightAngle

Why this choice
---------------
- RCJ-01X is a long-running manufacturer family with a published mechanical drawing.
- RCJ-011 through RCJ-017 share the same PCB pattern; the final digit is color.
- RCJ-012/013 are broadly stocked by major distributors, so the design is not tied to
  one obscure JLC-only connector.
- The two outputs remain electrically identical mono outputs, each through its existing
  100-ohm isolation resistor, matching the original dual-RCA circuit.

Footprint source
----------------
The footprint uses the manufacturer recommended PCB layout:
- electrical pad 1 at (0, 0), drill 2.6 mm
- electrical pad 2 at (5.0, 0), drill 2.6 mm
- duplicate electrical pad 1 at (10.0, 0), drill 2.6 mm
- non-plated board-lock hole at (5.0, -4.5), drill 1.7 mm

The pad/hole coordinates are taken from the CUI/Same Sky RCJ-01X datasheet.
The F.Fab/Courtyard body outline is conservative and should be checked against your
actual PCB edge/enclosure placement before fabrication.

KiCad
-----
Keep fp-lib-table and the Odderon.pretty folder beside the .kicad_sch file.
KiCad will resolve the footprint as a project-specific library.
