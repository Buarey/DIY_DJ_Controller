# Open Source Publishing Checklist

Use this checklist before making the GitHub repository public or announcing it.

## Repository

- Add the license files and `LICENSE.md` overview.
- Keep generated files out of commits: KiCad backups, `fp-info-cache`, `.kicad_prl`, PlatformIO build output, and `.DS_Store`.
- Confirm no personal files, credentials, private notes, or unfinished exports are tracked.
- Push the open-source preparation commit.

## GitHub Settings

- Set the repository visibility to public when ready.
- Enable Issues.
- Enable Discussions if you want build-help conversations separate from bug reports.
- Add topics: `diy-electronics`, `dj-controller`, `midi-controller`, `mixxx`, `platformio`, `arduino`, `kicad`, `open-hardware`, `3d-printing`.
- Add labels: `firmware`, `hardware`, `pcb`, `3d-models`, `mapping`, `docs`, `bug`, `enhancement`, `good first issue`, `help wanted`, `safety`.

## First Release

- Tag the current working Mixxx prototype as `v1.0.0`.
- Attach or link the firmware source, Mixxx mapping files, STL files, wiring images, and build notes.
- State that Rekordbox is experimental/unsupported for the current hardware revision.
- Mention known issues, especially swapped jog assignment and prototype hand-wiring.

## Community

- Create 3-5 starter issues that are genuinely approachable.
- Add one pinned issue for build reports.
- Ask contributors to include photos and version details when reporting hardware problems.
