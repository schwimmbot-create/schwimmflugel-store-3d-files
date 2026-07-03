# Schwimmflugel Store — 3D Files

This repository holds the source 3D CAD files for digital products sold
on [Schwimmflugel Designs](https://schwimmflugel.local/store/) under the
**3D Files** filter.

Every folder here is a standalone product. Releases are tagged per
product (`<slug>-v<MAJOR>.<MINOR>.<PATCH>`), so the URL on each store
card points at the exact commit a buyer can verify before downloading.

## What you'll find here

- STL files ready for slicing
- STEP files for CAD re-edits and parametric tweaking
- Print profiles and recommended settings where they matter

## What's NOT here

- Firmware (lives in
  [schwimmflugel-store-firmware](https://github.com/schwimmbot-create/schwimmflugel-store-firmware))
- Rendered images (those live on the store product cards, generated
  from MiniMax editorial-style product photography)

## License

3D files in this repository are released under **CC-BY-4.0**
([LICENSE](./LICENSE)). You can:

- Use them in personal and commercial builds
- Modify, remix, and redistribute
- Sell prints made from them

The only requirement is attribution. The README inside each product
folder spells out what credit to give and where.

## Releases and tags

Each product gets its own semver tag, e.g. `robotics-mount-bracket-v1.0.0`.
The store card URL points at the release page, not the latest commit, so
buyers always know which version they downloaded.

If a release breaks something (bad geometry, slicer issue, etc.), the
fix lands as `<slug>-v1.0.1` — v1.0.0 stays available because someone
may already be mid-print on those files.

## Repo layout

```
schwimmflugel-store-3d-files/
├── LICENSE
├── README.md
├── robotics-mount-bracket/
│   ├── README.md
│   ├── robotics-mount-bracket.stl
│   ├── robotics-mount-bracket.step
│   └── print-profile.md
└── project-enclosure/
    ├── README.md
    ├── project-enclosure-top.stl
    ├── project-enclosure-bottom.stl
    └── print-profile.md
```

## Questions or issues with a file?

Open an issue on this repo, or use the contact form on
[schwimmflugel.local](https://schwimmflugel.local/contact/). Include the
release tag you're working from.