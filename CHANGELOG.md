# Release notes

These notes describe local app builds. No binaries or source archives are published here.

## 2.25.2-alpha.1

Add color from image now uses a resizable zoomable preview with plus/minus, Fit, mouse-wheel magnification, drag panning and scrollbars. Original image detail is retained rather than a small thumbnail. Click selection accounts for the displayed image coordinates; dragging does not pick another color. Overlay refresh preserves zoom. Selection controls sit beside the image.

Validation: 69 automated tests and packaged checks passed. New packaged checks exercise zoomed canvas selection and drag without reselection. App files remain local.

## 2.25.1-alpha.1

Fixed swap-guide lines to include the selected library filament's brand, line, color name and TD alongside the editable stage label and hex. Manual text guides and native 3MF embedded guides share this behavior, including picked/painted stages and borders. Custom swatches are labeled Custom color. Existing exported guides require re-export from the saved project.

Validation: 69 automated tests passed, including explicit library-name assertions for generic stage labels, painted stages, borders and custom labels in both guide formats. Packaged application checks passed. App files remain local.

## 2.25.0-alpha.1

Fixed filament library mouse-wheel routing: the list scrolls independently, while the surrounding editing form scrolls under the pointer even in the modal assignment picker. Use and Close stay fixed at the bottom.

Added Duplicate filament. It saves the displayed values as a starred personal copy with a fresh identity and unique copy name, selects it for editing, and leaves the original unchanged. Catalog IDs are not reused. Renamed Product / range to Filament line with examples Hyper PLA and PLA Matte.

Validation: 68 automated tests passed. Packaged checks verified list/form scrolling in a grabbed dialog, independent duplicate creation and existing project/export flows. User validation remains pending. App files remain local; only tracking text is published.

## 2.24.0-alpha.1

Added Help > Advanced Relief Tutorial with eight steps for personal filaments, painting, layer counts, connected-area raising, borders and native export checks. Navigation does not change work.

Added File > New relief, Ctrl+N and a main-window button. Save/Discard/Cancel protects current work; canceling or failing the save keeps the existing project. Library and preferences are retained.

HEIC/HEIF/HIF import uses a bundled decoder, with no separate Windows image extension required. Imports the primary still image with orientation into 8-bit RGB; motion/depth/HDR information is not retained. Known-filament descriptions hide the unspecified-product placeholder without deleting metadata.

3D inspection now offers Fast (100), Detailed (200, default) and Fine (400) longest-axis sample limits, bounded by export spacing. Dragging uses fast geometry and restores chosen detail on release. Export geometry/settings are unchanged.

Validation: 67 automated tests passed, including HEIC decode and preview-resolution bounds. Packaged checks passed for decoder availability, tutorial navigation and New relief cancellation/reset, plus existing project/export coverage. Physical print and clean-machine checks remain pending. Only tracking text is published; app files remain local.

## 2.23.0-alpha.1

Added 42 MarsWork PLA Basic/Matte website swatches and 15 Creality measured-swatch entries, for 1,017 catalog records. Each new record includes its source URL. Existing personal records remain intact. Sources: [MarsWork Basic](https://www.marswork3d.com/products/pla-basic), [MarsWork Matte](https://www.marswork3d.com/products/pla-matte), and [FilamentColors Creality measurements](https://filamentcolors.xyz/library/manufacturer/177/).

Assigned filament buttons now show the color name and TD status. Picker, border and painting descriptions include product/range. New entries retain unknown TD rather than guessed values; blank TD is supported in the library, projects and export metadata. Website swatches are not calibrated print measurements; independent measurements are not manufacturer guarantees.

Validation: 64 automated tests and packaged GUI/project/export checks passed. Physical print validation remains pending. App source, catalog and installers remain local.

## 2.22.0-alpha.1

Added File > Filament library and a main-window library button. Save catalog or new filaments to a persistent personal library; starred entries sort first and can be unstarred. Assignment, border and paint color pickers suggest personal filaments and display their known TD. Painting optionally auto-matches sampled colors to personal filaments.

Suggestions rank by digital RGB proximity. An optional preferred TD breaks ties between equally close colors; this is not a calibrated prediction of the best printed color or TD. Known filament identity remains attached to assignments.

Validation: 63 automated tests and packaged GUI/project checks passed. Physical print validation remains pending. Source, catalog data and builds stay local.

## 2.21.0-alpha.1

Integrated the known-filament library and supplied 960-profile catalog into the main app. Add/edit brand, product, material, color name, hex, TD in millimeters and source notes. Assignment, painting and border pickers provide library selection plus direct six-digit hex editing with a live swatch. Project assignments are independent copies. Custom hex clears known-filament identity. Same-hex filaments with different identity or TD remain separate in native CFS slots, combining, connected selection and compact parts. Native exports include a filament-record manifest.

TD is stored only in this step; no optical prediction or optimization was added to the main app. Library material identity does not automatically choose printer temperature profiles. Supplied TD values remain unverified.

Validation: 61 automated tests and packaged GUI/project checks passed. Main Windows build includes the catalog. Physical slicer/print validation remains pending. Source, data and builds remain local.

## 2.20.0-alpha.1

Added Raise connected color area in detected-color mode. Click the assigned-color preview to highlight a connected line or region, including diagonal neighbors. Zoom and pan help with thin lines. Set layers above the current highest artwork stage; the selected area becomes an independent top stage using the existing filament slot. Other artwork stage heights remain unchanged. A separate raised border follows the new artwork height. This first version does not support arbitrary local offsets within intervening filament bands. Frozen masks and counts persist in .relief projects and Undo/Redo; the 16-stage limit remains.

Validation: 57 automated tests passed, including disconnected same-color regions, diagonal connectivity, mask restoration and watertight raised geometry. Packaged checks exercised click selection, three added layers, save/open and Undo/Redo. Physical print validation pending. App files remain local.

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
