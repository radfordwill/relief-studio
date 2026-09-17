# Feature status

Implemented means available in a local build. Physical-print and clean-machine validation are tracked separately.

| Feature | Status | Evidence / limits |
|---|---|---|
| Image import, grayscale heightmap, contrast and inversion | Implemented | Successful user test prints |
| Width, height, relief depth and solid backing | Implemented | Single-mesh STL/3MF export |
| Automatic color detection and editable filament stages | Implemented | User-confirmed multicolor prints; individual printer configurations still need testing |
| Pick and recolor connected or matching image regions | Implemented | Selections retained in projects and exports |
| Border color, width and height | Implemented | User-confirmed white-border print |
| Individual stage layer counts and color-count warnings | Implemented | Broader custom-count print validation pending |
| Grayscale/custom color scales and two-height/two-layer modes | Implemented | Broader physical validation pending |
| Native Creality CFS 3MF and bundled printer profiles | Implemented | Automatic filament assignments; broader profile testing pending |
| Save/open .relief projects, Undo/Redo, original image reload | Implemented | Automated and packaged app checks |
| Preview zoom, pan and 3D orbit | Implemented | Packaged app checks; usability feedback remains useful |
| Help, first-print tutorial, themes and About | Implemented | Packaged app checks |
| Windows installer and .relief association | Implemented | Clean-machine install/upgrade/uninstall validation pending |
| Fine 0.25 mm default detail and surface detail inside color bands | Implemented, 2.17 | Mesh checks passed; comparison prints pending |
| Compact relief | Experimental, 2.17 | Requires compatible repeats of the first filament color; separate aligned STL parts export, manual slicer material assignment |
| Filament library with 960 supplied profiles | Local TD development | 41 brands; supplied values not independently verified |
| Transmission-distance preview | Experimental local TD development | Uncalibrated approximation; no print-color guarantee |

STL itself does not store filament assignments. The regular native CFS 3MF export carries them. The experimental compact workflow exports aligned material parts with a color manifest instead.

## 2.18.0-alpha.1 — Existing print colors

Painting, row assignments and borders can select a named existing print color. Native CFS 3MF shares identical-color filament slots while retaining separate height stages. Adjacent matching stages need no tool change. Assignments copy colors; later edits are independent. 49 automated tests and packaged picker checks passed; physical slicer/print validation pending.

## 2.18.0-alpha.2 — Closest assigned colors

Painting now automatically picks the nearest assigned filament by RGB distance. Manual choices disable automatic matching until re-enabled. Border and assignment pickers rank matches and offer Use closest match. Matching uses digital swatches, not optical print predictions. 50 automated tests and packaged app checks passed.

## 2.19.0-alpha.1 — Combine matching stages

Matching paint colors can combine into existing height stages. Height changes require Yes/No confirmation; No retains a separate stage sharing the filament slot. Existing artwork rows can combine, and borders can use an artwork-stage height. Projects retain the choices. 54 automated tests and packaged checks passed; physical slicer/print validation remains pending.
