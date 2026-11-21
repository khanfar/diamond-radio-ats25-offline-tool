# Diamond Radio ATS-25 Offline Tool 1.2.0

This release refreshes every bundled ATS-25 firmware image while retaining the complete offline installer, backup, restore, maintenance, and EiBi Manager functions.

## New in 1.2.0

- Updated **Diamond Radio v1.1.1 BETA** images for ILI9341, ST7789 Pro+ AIR, ILI9488 Mega, and Ultra.
- On-radio **NAVTEX** decoding with channel presets, live spectrum and tone markers, adjustable tuning, message logging, and PC Control USB integration.
- VHF AIR coverage updates for supported Pro+ AIR and Ultra hardware.
- Additional radio-screen waterfall and 3D display choices.
- Ultra NAVTEX display update corrected to prevent the repeated black flicker reported by testers.
- Updated standalone firmware downloads match the images embedded in the EXE.

## Existing functions retained

- Automatic full backup before bundled installation, with an explicit skip option.
- Custom BIN installation at a user-selected address.
- Full flash backup and restore.
- Separate Settings and Memories/EiBi backup and restore.
- Fully offline EiBi Manager with 9,541 embedded station records.
- Reset, guarded full-flash erase, live logs, progress display, and write verification.

## Download

- **Windows ZIP:** recommended; includes the EXE, read-me, and legal notices.
- **Standalone EXE:** the complete offline tool, including firmware and EiBi data.
- **Separate firmware files:** optional manual downloads. The same files are already embedded in the EXE.
- **License ZIP:** bundled firmware, EiBi, and application notices.
- **SHA256SUMS.txt:** hashes for checking every downloaded release file.

## Use

Connect the radio, select its COM port, and click **CONNECT**. Make a full backup, select the exact display family, accept the license, and choose **INSTALL DIAMOND RADIO**. Keep USB and power connected until installation and verification finish.

For NAVTEX after installation, open the radio's decoder menu and select NAVTEX, or use Diamond PC Control over USB. No audio cable is required for radio-side or USB decoding. Accurate USB tuning, a suitable antenna, and a moderate receiver volume are important; adjust during an active transmission for stable lock and few errors.

Version 1.2.0 passed package integrity and frozen-executable self-tests. Its NAVTEX firmware was tested on ATS-25 and Ultra hardware. Older releases, including v1.1.0 and v1.0.0, remain available. This repository contains binary releases and notices only; Diamond-specific source code is not distributed.
