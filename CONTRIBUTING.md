# Contributing

Thanks for wanting to help with this DIY DJ controller. The project is especially useful when people contribute practical build feedback: firmware behavior, Mixxx mappings, PCB notes, enclosure fixes, photos, and clear documentation.

## Good First Contributions

- Improve build instructions or add missing photos.
- Report parts that did or did not fit the 3D-printed enclosure.
- Test the Mixxx mapping on another operating system.
- Confirm replacement potentiometers, encoders, buttons, or Pro Micro clones.
- Fix firmware comments or MIDI mapping documentation.
- Add clear notes from a real build attempt.

## Before You Start

Open an issue before large changes, especially for PCB redesigns, v2 hardware, USB audio work, or mapping changes that affect existing controls. Small docs fixes can go straight to a pull request.

Please keep changes focused. A pull request should usually touch one area: firmware, Mixxx mapping, Rekordbox reference, PCB, 3D models, or docs.

## Development Setup

Firmware uses PlatformIO:

```bash
cd CDJ_firmware
pio run
```

The current build target is `sparkfun_promicro16`.

For Mixxx mapping changes, test with:

- `controllers/mixx_Mapping/DJC-DIY.midi.xml`
- `controllers/mixx_Mapping/DJC-DIY-scripts.js`

For hardware changes, use the project files under `PCB/DYI_CDJ_v1/` and keep generated KiCad backup/cache files out of commits.

## Pull Request Checklist

- Describe what changed and why.
- For firmware changes, run `pio run` from `CDJ_firmware/`.
- For mapping changes, describe the tested Mixxx or Rekordbox version.
- For PCB changes, include the KiCad version and note whether ERC/DRC was checked.
- For 3D model changes, include print orientation/material notes when relevant.
- Update `README.md` if the source of truth, wiring, parts list, or build behavior changed.
- Do not include local caches, KiCad backup zips, generated build output, or `.DS_Store` files.

## Licensing

By contributing, you agree to license your contribution under the same license as the files you change:

- Software and controller mappings: `GPL-3.0-only`
- Hardware, PCB, wiring, and 3D design files: `CERN-OHL-S-2.0`
- Documentation and media: `CC-BY-4.0`

If your contribution includes third-party material, mention its source and license in the pull request.
