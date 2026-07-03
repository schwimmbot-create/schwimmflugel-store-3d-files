# Print Profile — Project Enclosure (Two Halves)

Tested on Prusa MK4 with PrusaSlicer 2.7. The two halves ship as
separate STLs because the orientation is different for each.

## Bottom half (project-enclosure-bottom.stl)

| Parameter | Value | Notes |
|---|---|---|
| Material | PETG (eSun PETG black) | ABS also tested |
| Layer height | 0.2 mm | |
| Infill | 25% gyroid | Bosses are reinforced — gyroid keeps them rigid |
| Perimeters | 4 | |
| Top/bottom layers | 5/4 | |
| Orientation | Flat side down | Bosses print vertical, clean threads |
| Brim | 6 mm | Helps with the larger flat face |
| Support | None | Bosses and pass-throughs are overhang-friendly |

## Top half (project-enclosure-top.stl)

| Parameter | Value | Notes |
|---|---|---|
| Material | PETG (eSun PETG black) | Same as bottom for matched finish |
| Layer height | 0.2 mm | |
| Infill | 25% gyroid | |
| Perimeters | 4 | |
| Top/bottom layers | 5/4 | |
| Orientation | Vented side up (lid face up) | Vent slots print cleanly in this orientation |
| Brim | None | Small enough flat face to avoid warp |
| Support | None | Lid vents are designed to print without supports |

## Assembly

The two halves mate with **M3×8 mm countersunk screws** through the
four bosses in the bottom shell.

Tighten in a cross pattern (1 → 3 → 2 → 4) to avoid warping the lid
against the bottom. Don't overtighten — PETG bosses will strip if you
push past 0.4 N·m.

## Cable pass-through

The rectangular cutout on the rear edge of the bottom shell is sized
for a PG7 cable gland (fits 3-6.5 mm cable). For other cable sizes,
swap the gland rather than reprinting.

## Tested PCBs

The interior is sized for a 60×40 mm PCB with 10 mm of clearance on
each side. If your PCB is larger, the next size up enclosure is
planned as `project-enclosure-large-v1.0.0` — open an issue on the
repo if you want to be notified when it's released.

— Schwimmflugel Designs