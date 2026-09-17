# Release notes

These notes describe local app builds. No binaries or source archives are published here.

## 2.19.0-alpha.1

Matching paint colors can combine into existing height stages. Height changes require Yes/No confirmation; No retains a separate stage sharing the filament slot. Existing artwork rows can combine, and borders can use an artwork-stage height. Projects retain the choices. 54 automated tests and packaged checks passed; physical slicer/print validation remains pending.

## 2.18.0-alpha.2

Painting now automatically picks the nearest assigned filament by RGB distance. Manual choices disable automatic matching until re-enabled. Border and assignment pickers rank matches and offer Use closest match. Matching uses digital swatches, not optical print predictions. 50 automated tests and packaged app checks passed.

## 2.18.0-alpha.1

- Existing print-color swatches available for painting, row assignments and borders.
- Native CFS exports reuse identical-color slots and skip redundant adjacent tool changes.
- Painting retains a chosen filament when selecting another source area; preview reports unique slot count.
- 49 automated tests and packaged checks passed; installer compiled. Physical slicer/print validation pending.

## 2.17.0-alpha.2

- Removed external product comparisons from app text, help and export instructions.
- Clarified compact relief eligibility and its separate export workflow.
- Packaged app checks passed.

## 2.17.0-alpha.1

- Fine 0.25 mm default detail for new images.
- Optional surface detail within color bands while preserving stage boundaries.
- Experimental compact relief suggestions, selection, height comparison, 3D inspection and aligned per-filament STL export.
- 47 automated tests and packaged checks passed. Physical compact-print validation remains pending.

## 2.16.0-dev.2 — separate local TD development

- Added the supplied 960-profile filament catalog spanning 41 brands.
- Search and saved overrides for filament identity, color, material and transmission distance.

## 2.16.0-dev.1 — separate local TD development

- Editable filament library and per-stage TD assignments.
- Experimental thickness-aware blended preview; calibration pending.

## 2.15 series

- Pick source colors and recolor matching or connected regions.
- Warn before exceeding eight color stages, including the border.
- Improved preview panning and single-step stage arrows.

## Earlier delivered features

- App artwork and About credits; grayscale/custom scales and two-layer modes.
- Guided first-print tutorial; 3D orbit, preview zoom/pan, Undo/Redo and image reload.
- Bundled printer profiles, help, light/dark modes and alpha version labels.
- Windows installer, project association, saved projects and editable stage layer counts.
- Image-to-relief export, automatic color detection/assignment and editable borders.

Earlier issue numbers belonged to the replaced repository and are not reused as evidence here.
