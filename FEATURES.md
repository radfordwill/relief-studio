# Relief Studio development tracker

Use one row per feature or bug. Status flow: Idea → Planned → In progress → Testing → Released.
Released means included in a build; record user/print validation separately.

| ID | Feature | Status | Version | Validation / next step |
|---|---|---|---|---|
| [RS-001](https://github.com/radfordwill/relief-studio/issues/1) | Grayscale relief, solid backing, STL/3MF/PNG | Released | Existing | User confirmed successful prints |
| [RS-002](https://github.com/radfordwill/relief-studio/issues/2) | Color detection, assignments and native Creality CFS export | Released | Existing | User confirmed multicolor print; broader printer testing pending |
| [RS-003](https://github.com/radfordwill/relief-studio/issues/3) | Border color, width and height | Released | Existing | User confirmed white-border print |
| [RS-004](https://github.com/radfordwill/relief-studio/issues/4) | Save/open embedded-image .relief projects | Released | 2.8 | Automated and packaged smoke tests |
| [RS-005](https://github.com/radfordwill/relief-studio/issues/5) | Individual color layer counts | Released | 2.8 | Automated tests; physical custom-count print pending |
| [RS-006](https://github.com/radfordwill/relief-studio/issues/6) | Installer and Windows project association | Released | 2.9 | Installer compiled; clean-machine install/uninstall test pending |
| [RS-007](https://github.com/radfordwill/relief-studio/issues/7) | In-app feature guide | Released | 2.10.0-alpha.1 | Packaged GUI smoke test; user readability review pending |
| [RS-008](https://github.com/radfordwill/relief-studio/issues/8) | Persistent light/dark appearance | Released | 2.10.0-alpha.1 | Both modes exercised in packaged GUI; user visual review pending |
| [RS-009](https://github.com/radfordwill/relief-studio/issues/9) | Alpha version labeling | Released | 2.10.0-alpha.1 | Main title, About, help and installer version |
| [RS-010](https://github.com/radfordwill/relief-studio/issues/10) | Clean-machine installation and association validation | Planned | Unscheduled | Install, double-click path with spaces, repair, upgrade and uninstall |
| [RS-011](https://github.com/radfordwill/relief-studio/issues/11) | Filament transparency / transmission calibration | Idea | Unscheduled | Define calibration workflow before implementation |
| [RS-012](https://github.com/radfordwill/relief-studio/issues/12) | Optical printed-color simulation | Idea | Unscheduled | Needs calibrated filament data |
| [RS-013](https://github.com/radfordwill/relief-studio/issues/13) | Native Bambu AMS export | Idea | Unscheduled | Needs supported printer/profile scope and validation |

For each new bug record: app version, Windows/slicer version, steps, expected
result, actual result, and a sample .relief project or screenshot when useful.
Assign a priority and target release before starting work. Update this tracker
and CHANGELOG.md with each release. Ideas are suggestions, not commitments.

When moving to GitHub, turn IDs into Issues and use a Project board with the
same statuses. Keep release milestones and a separate validation checklist.
