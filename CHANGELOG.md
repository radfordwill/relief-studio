# Release history

## 2.13.0-alpha.1 — 2026-09-11

- Added Help > First Print Tutorial with eight scrollable steps, Back/Next and action buttons.
- Covered image setup, dimensions, colors, profiles, preview/border, .relief save, native CFS 3MF export and slicer checks.
- Added remembered Don't show at startup option; direct project-file launches skip startup display.
- Navigation does not modify work or assume successful saving/export. Loading a replacement image from the tutorial asks before replacing existing work.
- Added preference preservation tests and packaged walkthrough/action-routing checks.

## 2.12.0-alpha.1 — 2026-09-11

- Added software-rendered 3D grayscale and color relief orbit previews.
- Added drag rotation, right-drag pan, wheel zoom, four preset views and Fit.
- Added Refresh and clearly labeled display-only height exaggeration.
- Reduced preview mesh detail independently of export detail; includes backing and color borders.
- Added geometry/rendering tests and packaged UI coverage. No new print validation required for view-only geometry changes; user interaction review remains pending.

## 2.11.0-alpha.1 — 2026-09-11

- Bundled versioned Creality CFS printer/PLA profiles with their inherited dependencies, license and source notice.
- Added 20-change Undo/Redo for settings, palettes, filament order and borders.
- Added zoom, Fit, scrollbars and drag panning to both previews.
- Added undoable Reload original image using the embedded source.
- Updated Help and packaging for offline profile availability.
- Automated and packaged verification recorded in GitHub issues #16–19. Physical printing and clean-machine installer validation remain open.

## 2.10.0-alpha.1 — 2026-09-10

- Added Help > Feature guide, with seven selectable topics and scrollable explanations.
- Added View > Dark mode and the same toggle in File > Settings.
- Remembered appearance across launches without overwriting printer preferences.
- Preserved filament swatch and image colors when switching appearance.
- Marked the app, help and installer as alpha; central app version lives in version.py.
- Added a development feature tracker and updated the installer workflow.

## 2.9

- Added a per-user Windows 11 installer, shortcuts and uninstall support.
- Added .relief file registration on install and repair through File > Settings.
- Opened saved projects passed from Windows Explorer.

## 2.8

- Saved complete .relief projects with embedded source images.
- Added individual color layer counts.

Earlier feature and validation notes remain in README.md.

