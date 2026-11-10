# Diamond Radio ATS-25 Offline Tool 1.0.0

First public release of the standalone offline Windows installer and maintenance tool for ATS-25-family radios.

## Included

- Bundled Diamond Radio **v1.1.1 BETA** installation for ILI9341, ST7789, ILI9488, and Ultra display families.
- Automatic full backup before bundled installation, with an explicit skip option.
- Custom BIN installation at a user-selected address.
- Full flash backup and restore.
- Separate Settings and Memories/EiBi backup and restore.
- Reset, guarded full-flash erase, live logs, progress display, and write verification.
- Embedded firmware and tools: no website, internet connection, Python installation, or account is required.

## Download

- **Windows ZIP:** recommended; includes the EXE, read-me, and legal notices.
- **Standalone EXE:** the complete offline tool.
- **Separate firmware files:** optional manual downloads. The same files are already embedded in the EXE.
- **License ZIP:** bundled firmware and application notices.
- **SHA256SUMS.txt:** hashes for checking every downloaded release file.

## Use

Connect the radio, select its COM port, and click **CONNECT**. Make a full backup before writing or erasing anything. Select the exact display family for bundled installation, accept the License Agreement, and keep USB and power connected until verification finishes.

Use address **0x0** for full images and **0x10000** only for compatible app-only images. Full erase removes everything; keep a verified backup.

This repository contains binary releases and notices only. Diamond-specific source code is not distributed.
