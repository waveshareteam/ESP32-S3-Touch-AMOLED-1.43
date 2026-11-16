# 05_WIFI_AP

[English](README.md) | [简体中文](README_ZH.md)

## What It Does

Creates a 2.4 GHz Wi-Fi access point.

## Hardware Required

ESP32-S3-Touch-AMOLED-1.43 development board and a USB data cable. Use a phone or computer with Wi-Fi to find the access point.

## How to Run

Open an ESP-IDF terminal in this directory and run with a version listed in the repository README:

```bash
idf.py set-target esp32s3 build flash monitor
```

## Expected Result

The access point appears in the Wi-Fi network list and accepts client connections.

## Troubleshooting

The default SSID is `waveshare_esp32` with password `wav123456`; edit the access-point settings in the source and upload again.
