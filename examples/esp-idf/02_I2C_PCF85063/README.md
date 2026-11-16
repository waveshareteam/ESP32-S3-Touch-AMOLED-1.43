# 02_I2C_PCF85063

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Sets and reads the onboard PCF85063 RTC over I2C.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The log repeatedly prints the RTC date and time.

## Troubleshooting

The demo writes a fixed initial date and time on every boot; change it in the RTC example before using it as a clock.
