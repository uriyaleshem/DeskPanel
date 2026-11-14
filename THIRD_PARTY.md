# Third-party source and assets

- Waveshare hardware sources: copyright notices preserved in copied source files. Exact official repository/commit and paths in [HARDWARE.md](docs/HARDWARE.md). No substituted generic board drivers.
- ESP-IDF 5.5.1: Espressif, Apache-2.0 and component-specific licenses, downloaded by the bootstrap script.
- LVGL 9.4.0: MIT, downloaded by ESP-IDF component manager; lock includes hash.
- Espressif adapter/touch and dependencies: registry package licenses accompany downloads.
- Heebo, Noto Sans Symbols and Noto Sans Symbols 2: SIL Open Font License 1.1. TTFs and OFL files in `desktop/app/resources/`. Generated LVGL bitmaps derive from these bundled fonts.
- Windows zone mapping: Unicode CLDR release-47 `windowsZones.xml`, world mapping (`territory=001`), Unicode license. [Source](https://github.com/unicode-org/cldr/blob/release-47/common/supplemental/windowsZones.xml), [license](https://www.unicode.org/license.txt).
- Python/Qt/OAuth libraries: pinned in requirements-lock.txt; PySide6/Qt distribute their license data in the bundle. Review dependency licenses before redistributing a modified commercial package.
- Utility SVG icons are original small path drawings included in this project.

Asset and vendor SHA-256 values are recorded in `shared/provenance.json` for reproducibility.

DeskPanel's 8 October 2026 display modifications are recorded in `firmware/patches/display.cmake`: derived build copies fix ESP LVGL adapter 0.5.2 dirty-region CPU rotation, add an ESP-IDF RGB DMA-underrun counter, and set the Waveshare panel initialization clock to 18MHz. Original source/license notices remain intact. Managed downloads and checked-in vendor reference files are not edited; generated sources are included in the firmware binaries under their original licenses.
