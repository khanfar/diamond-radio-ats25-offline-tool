# Diamond Radio ATS-25 Offline Tool 1.1.0

This tested update adds a completely offline EiBi Database Manager while retaining all installer, backup, restore, and maintenance functions from version 1.0.0.

## New in 1.1.0

- **EiBi Manager tab** with the current broadcast schedule embedded directly in the application.
- **9,541 station records**, schedule dated **October 4, 2026**.
- **UPLOAD EiBi DATABASE** replaces the radio's schedule without requiring the website or an internet connection.
- Live percentage and byte progress, followed by radio confirmation and automatic restart.
- **DELETE DATABASE** removes only the EiBi schedule. Station memories, settings, and firmware are not changed.
- Database integrity checking and clear compatibility guidance.

## Existing functions retained

- Bundled Diamond Radio **v1.1.1 BETA** installation for ILI9341, ST7789, ILI9488, and Ultra display families.
- Automatic full backup before bundled installation, with an explicit skip option.
- Custom BIN installation at a user-selected address.
- Full flash backup and restore.
- Separate Settings and Memories/EiBi backup and restore.
- Reset, guarded full-flash erase, live logs, progress display, and write verification.

## Download

- **Windows ZIP:** recommended; includes the EXE, read-me, and legal notices.
- **Standalone EXE:** the complete offline tool, including firmware and EiBi data.
- **Separate firmware files:** optional manual downloads. The same files are already embedded in the EXE.
- **License ZIP:** bundled firmware, EiBi, and application notices.
- **SHA256SUMS.txt:** hashes for checking every downloaded release file.

## Use EiBi Manager

Connect the radio, select its COM port, and click **CONNECT**. Open **EiBi Manager**, then choose **UPLOAD EiBi DATABASE**. Keep USB and power connected until completion. The radio restarts automatically after a successful upload; open its EiBi page to browse the stations.

**DELETE DATABASE** affects only the EiBi schedule. You can upload the embedded database again at any time.

Version 1.1.0 was hardware-tested with EiBi upload and deletion. Older releases remain available. This repository contains binary releases and notices only; Diamond-specific source code is not distributed.
