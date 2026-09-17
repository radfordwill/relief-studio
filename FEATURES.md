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
