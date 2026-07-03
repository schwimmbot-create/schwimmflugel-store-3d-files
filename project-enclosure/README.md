# Project Enclosure — Two Halves (STL Pack)

Two-piece 3D-printed enclosure for small bench electronics: top and
bottom shells with cable pass-throughs, M3 mounting bosses, and a
vented lid.

This is the **v1.0.0** release. Released under
[CC-BY-4.0](../../LICENSE).

## What's in this folder

| File | Format | Use it for |
|---|---|---|
| `project-enclosure-top.stl` | STL (ASCII) | Slicing the top half directly |
| `project-enclosure-bottom.stl` | STL (ASCII) | Slicing the bottom half directly |
| `project-enclosure.step` | STEP AP214 | Re-editing in Fusion 360 / SolidWorks / FreeCAD |

The two halves are designed to mate with M3×8 mm countersunk screws
through the four bosses in the bottom shell.

## Print settings (recommendation)

- **Material:** PETG or ABS for any electronics that may run warm
- **Layer height:** 0.2 mm
- **Infill:** 25% gyroid (the lid vents are functional; gyroid keeps
  the vent geometry clean)
- **Perimeters:** 4

See [`print-profile.md`](./print-profile.md) for the full slicer notes.

## STEP file note

`project-enclosure.step` includes both halves as a single assembly so
you can edit the dimensions parametrically and re-export a matched
pair. If your CAD tool chokes on the simplified assembly, the two
STLs are independent and can be edited standalone.

## Use and attribution

You can print, modify, and sell enclosures made from these files.

Attribution: credit **Schwimmflugel Designs** with a link to
https://github.com/schwimmbot-create/schwimmflugel-store-3d-files.

## Versioning

This folder is released as `<slug>-v<MAJOR>.<MINOR>.<PATCH>`. v1.0.0
ships the two halves at the dimensions verified on the bench with the
60×40 mm PCB it was designed around. Fixes and PCB-cutout changes
land as v1.0.1, v1.1.0, etc. The previous tag always stays available.