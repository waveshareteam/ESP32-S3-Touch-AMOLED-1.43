# Firmware

[English](README.md) | [简体中文](README_ZH.md)

Ready-to-flash firmware tested on the ESP32-S3-Touch-AMOLED-1.43 board. Each file is a merged image flashed at `0x0`; the date (or upstream version) in the file name is its version.

| File | Purpose |
| --- | --- |
| `ESP32-S3-Touch-AMOLED-1.43_FactoryOnly_20250305.bin` | Factory firmware, restores the out-of-box demo |

Flash with esptool:

```bash
python -m pip install esptool
python -m esptool --chip esp32s3 --port <PORT> erase-flash
python -m esptool --chip esp32s3 --port <PORT> write-flash 0x0 ESP32-S3-Touch-AMOLED-1.43_FactoryOnly_20250305.bin
```

The factory firmware source is in [`examples/factory`](../examples/factory/).
