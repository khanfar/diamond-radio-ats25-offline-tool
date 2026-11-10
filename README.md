# Diamond Radio ATS-25 Offline Tool

Official offline Windows installer and maintenance tool for **Diamond Radio ATS-25-family radios**.

- Product and Diamond-specific modifications: **M Khanfar**
- Distribution: **freeware**; Diamond-specific source code is not distributed
- Official website: **[diamondradio.web.app/install.html](https://diamondradio.web.app/install.html)**
- Current tool version: **1.1.0**
- Bundled firmware: **Diamond Radio v1.1.1 BETA**

## Download

Open **[Releases](https://github.com/khanfar/diamond-radio-ats25-offline-tool/releases/latest)** and choose:

- **DiamondRadio-ATS25Tool-v1.1.0-Windows.zip** — recommended package with the EXE, usage information, and legal notices.
- **DiamondRadio-ATS25Tool.exe** — standalone Windows application.

No Python installation, account, internet connection, or website access is needed to use the tool. All supported firmware images and the EiBi schedule database are already embedded in the EXE.

## Features

- Connect to an ATS-25-family radio and detect its ESP32 and flash capacity.
- Install the bundled firmware for the selected display/hardware family.
- Automatically make a full backup before bundled installation unless explicitly skipped.
- Install a custom BIN at a selected flash address.
- Make and restore complete flash backups.
- Save and restore Settings separately from Memories and the EiBi database without changing firmware.
- Upload the embedded EiBi schedule or delete only the EiBi database, with live progress and confirmation.
- Reset the radio or erase the entire flash with a typed confirmation.
- Follow live progress and diagnostic logs, with verification after every write.

## Supported bundled firmware

| Radio / display family | Separate firmware file |
| --- | --- |
| ATS-25 family and ATS-120 Pro — ILI9341 2.8-inch | `diamond-radio.bin` |
| ATS25 Pro+ AIR — ST7789 2.8-inch | `diamond-radio-st7789.bin` |
| ATS-Decoder Mega — ILI9488 3.5-inch | `diamond-radio-ili9488.bin` |
| ATS25 Ultra — ILI9488i 3.5-inch | `diamond-radio-ultra.bin` |

The release also provides these firmware files separately, together with `bootloader.bin` and `partitions.bin`, for manual use. They are optional downloads; the EXE already contains them.

## Quick start

1. Connect the radio using a USB data cable.
2. Open the tool, select the COM port, and click **CONNECT**.
3. Confirm that an ESP32 and the expected flash capacity are detected.
4. Make a **FULL BACKUP** before installation or maintenance.
5. To install bundled firmware, select the exact display family, accept the License Agreement, and click **INSTALL DIAMOND RADIO**.
6. Keep USB and power connected until installation and verification finish.

For a custom image, use **0x0** for a full-flash image or full backup. Use **0x10000** only for an app-only image over an existing compatible Diamond installation. An app-only file does not include the bootloader or partition table.

Full erase permanently removes firmware, settings, memories, and EiBi data. Keep a known-good full backup before using it.

Open **Licenses & Info → HOW TO USE / ALL CASES** inside the application for complete operating guidance.

## Legal and third-party notices

Diamond-specific source code is private. The application and bundled firmware are distributed as freeware. Third-party components retain their own licenses and copyright notices.

- [`DIAMOND_FREEWARE_NOTICE.txt`](DIAMOND_FREEWARE_NOTICE.txt)
- [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md)
- [`legal/`](legal/) — accompanying license texts

The software is provided without warranty. Always make a full backup before firmware installation or maintenance.
