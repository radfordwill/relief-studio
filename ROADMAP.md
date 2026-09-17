# Roadmap and validation

Priorities are planning notes, not promised release dates.

## Validate delivered work

- Compare fine-detail and textured relief prints against the original artwork, checking sharp edges, thin lines and useful height variation.
- Verify compact material parts in the slicer and with a physical print; inspect boundaries, backing, material assignments, print time and waste.
- Test installer, upgrade, uninstall and .relief association on a clean Windows 11 machine.
- Broaden printer/profile and custom-stage-layer-count validation.

## Planned investigation

- Edge-preserving cleanup and local shaping controls for better relief detail.
- Calibrate TD preview using known filaments and measured test prints before relying on predicted colors.
- Consider automatic assignments in a native multipart 3MF for compact relief.
- Evaluate native Bambu AMS export after defining supported printers and profiles.

## Current compact relief limits

The exact first filament color must recur later, and both runs must move consistently in the same brightness direction. A palette where each color appears once cannot nest. The flat color image may look unchanged; height changes appear in the comparison and 3D view. Compact changes apply only to the aligned-parts export. Most automatically detected palettes will not meet these conditions.
