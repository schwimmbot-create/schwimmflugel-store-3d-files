# Print Profile — Robotics Mount Bracket

Tested on a Prusa MK4 with PrusaSlicer 2.7. Other slicers should
translate cleanly.

## Recommended settings

| Parameter | Value | Notes |
|---|---|---|
| Material | PETG (eSun PETG black) | ABS also tested |
| Nozzle | 0.4 mm | |
| Layer height | 0.2 mm | 0.15 mm if you want a finer top surface |
| First layer height | 0.20 mm | Same as body — first layer is the flat reference face |
| Infill | 30% gyroid | Cubic also fine; gyroid gives better torsional resistance |
| Perimeters | 4 | Gives 1.6 mm wall — enough for the M3 boss area |
| Top/bottom layers | 5/4 | |
| Print speed | 60 mm/s outer, 80 mm/s inner | |
| Cooling | 50% from layer 4 | PETG needs some cooling; ABS turn off entirely |
| Brim | None | Flat face is large enough; no warping observed on Prusa MK4 |
| Support | None | Bracket is overhang-friendly in the orientation shipped |

## Orientation

Print **flat side down, mounting boss facing up**. This orientation
keeps the load path aligned with the layer lines and the boss lands
on the last layer (best surface finish on the boss face).

If your slicer reorients the model automatically, force the flat face
down by rotating the model before slicing.

## Alternate M3 bolt pattern

The v1.0.0 STL has the standard M3 bolt pattern on the boss face. If
you need a different pattern (e.g. M2.5 or M4), edit
`robotics-mount-bracket.step` in your CAD tool — the boss is a single
feature so the edit is quick.

## Post-processing

PETG: no post-processing needed.
ABS: light acetone-smoothing on the boss face if you want a polished
mounting surface. Skip on the rest of the bracket.

## Tested motors

- Standard-size hobby servo (40×20×36 mm case)
- NEMA-17 stepper (with separate collar — see note in main README)

If you're mounting something else, open an issue on the repo with the
motor dimensions and the load profile; I'll add a parameter note to
the next release if it's a common case.

— Schwimmflugel Designs